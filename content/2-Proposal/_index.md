---
title: "Proposal"
date: 2026-06-19
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# Playwright Automated Testing System using Docker on AWS

### 1. Executive Summary
The system is an End-to-End (E2E) automated testing platform for websites, designed to completely eliminate the need for engineers to manually monitor and run test suites upon every deployment. Playwright runs inside Docker containers to simulate real user behavior on web browsers (navigation, input, verifying display outputs), followed by an AI-powered summary step that translates raw technical logs into reader-friendly summaries sent via email.

The entire system runs on AWS under an event-driven, serverless-first architecture: Amazon EventBridge triggers scheduled test runs, Amazon SQS decouples test requests from execution, an AWS Lambda function (Coordinator) initiates a standalone Amazon ECS Fargate task for each test run, and the task automatically shuts down once the report generation is complete. Consequently, the system only incurs costs for the exact minutes the tests are executing, avoiding paying for a 24/7 server that remains idle most of the time. Administrative Dashboard access is managed through Amazon Cognito, supporting role-based access control with three roles (Admin, QA/Tester, Developer).

### 2. Problem Statement
**Current Problems**
Manual E2E testing requires testers to run scripts manually upon each deployment change, a workflow that cannot scale as the number of applications and test suites grows. There is no centralized system to schedule test runs, track historical Pass/Fail trends, or notify stakeholders automatically. Maintaining a continuous server just to be ready for the next test run generates wasted operational costs due to high idle time.

**The Solution**
The system supports two trigger sources: scheduled automatic runs via cron expressions (Amazon EventBridge) and on-demand manual triggers (Amazon API Gateway). Both sources are normalized into an Amazon SQS queue backed by a Dead Letter Queue (DLQ) to capture failed executions. An AWS Lambda function (Coordinator) acts as the queue consumer, calling the `RunTask` API to launch short-lived Amazon ECS Fargate tasks running Playwright tests packaged inside Docker images hosted on Amazon ECR. Upon completion, the task uploads HTML/JSON reports to a private Amazon S3 bucket, streams real-time logs to Amazon CloudWatch, and terminates itself.

A post-processing AWS Lambda function cleans up raw logs, filters out unnecessary info, and requests an external AI API to generate a natural language summary. The function includes a fallback mechanism to email the original reports directly if the AI call fails or times out. Amazon SES handles the final email notifications, including Pass/Fail counts, time-limited S3 Presigned URLs, and the AI-generated summary, delivering them to the registered recipient list of the targeted application.

**Benefits and Return on Investment (ROI)**
* **Elimination of Manual Testing**: No manual intervention or waiting around for test results.
* **Faster Response Time**: Converts a manual process that could take hours into an automated run completed in minutes.
* **Infrastructure Cost Optimization**: Charges are strictly pay-as-you-go based on actual run time instead of keeping a server active 24/7.
* **Comprehensive Historical Logging**: Every execution is permanently stored in Amazon DynamoDB for quality trend analysis, which is impractical with scattered Excel files.
* **Resource Optimization**: Frees up QA engineering resources to focus on designing higher-quality test suites rather than repeating manual verification scripts.

### 3. Solution Architecture
The system is divided into a Backend Engine (scheduling, executing, and reporting) and a Dashboard Console (UI tailored for Admin, QA/Tester, and Developer roles). All requests follow a single standardized pipeline with no bypasses (SQS -> Lambda Coordinator -> Fargate), whether triggered automatically or manually.

![Playwright Automation Testing Solution Architecture](/images/2-Proposal/playwright_architecture.png?featherlight=false&width=90pc)

**AWS Services Used**

| AWS Service | Role in Architecture |
| ----------- | -------------------- |
| **Amazon EventBridge** | Schedules and generates periodic test execution events (cron expressions). |
| **Amazon API Gateway (HTTP API)** | Receives manual trigger requests and dashboard API calls, authenticated via Lambda Authorizer. |
| **Amazon SQS + DLQ** | Buffers and normalizes test requests, with DLQ storing repeatedly failing runs. |
| **AWS Lambda (Coordinator)** | Consumes SQS messages and calls ECS `RunTask` to spin up Fargate tasks. |
| **Amazon ECS Fargate** | Runs Docker/Playwright containers within a Private Subnet, self-terminating upon completion. |
| **Amazon ECR** | Stores the Docker image containing the Playwright test runner. |
| **Amazon S3 (2 buckets)** | One bucket for static frontend Dashboard hosting; one private bucket for reports and test artifacts. |
| **Amazon CloudWatch** | Collects logs, metrics, and triggers alarms for task timeouts or DLQ message backlog. |
| **AWS Lambda (Post-processing)** | Cleans logs, queries the external AI API, and prepares notification emails. |
| **OpenAI API (External to AWS)** | Generates natural language log summaries (replacing Amazon Bedrock due to free tier constraints). |
| **NAT Gateway (Public Subnet)** | Allows the post-processing Lambda within the Private Subnet to access the external AI API. |
| **Amazon SES** | Sends email notifications directly to registered recipients. |
| **Amazon DynamoDB** | Stores test run history, Audit Logs, and system configurations. |
| **Amazon CloudFront** | Distributes static frontend files, integrated with AWS WAF CLOUDFRONT scope. |
| **Amazon Cognito** | Authenticates Dashboard users and issues tokens for role-based authorization. |
| **AWS Secrets Manager** | Securely stores AI API keys and other sensitive configuration secrets. |
| **Amazon VPC + VPC Endpoints (PrivateLink)** | Isolates Fargate tasks inside Private Subnets; AWS internal traffic does not traverse the public internet. |
| **AWS WAF (CloudFront + Regional scopes)** | Employs two Web ACLs to protect CloudFront distributions and API Gateway endpoints. |

**Component Design**
* **Trigger Layer**: EventBridge and API Gateway both push execution events to a shared SQS queue.
* **Execution Layer**: Lambda Coordinator launches an ECS Fargate task per run, which pulls the Playwright runner from ECR and runs headlessly in a Private Subnet.
* **Reporting Layer**: HTML/JSON reports are saved to a private S3 bucket, with real-time logs streamed to CloudWatch.
* **AI Layer**: A secondary Lambda processes the logs and sends them to the AI API via a NAT Gateway, backed by a circuit-breaker fallback to send original logs if the AI call fails.
* **Notification Layer**: SES emails reports to registered recipients along with time-limited S3 Presigned URLs.
* **Access Layer**: Cognito enforces unified role-based authorization (Admin, QA/Tester, Developer) at the API Gateway boundary.

### 4. Technical Implementation
**Implementation Phases**
The architecture has been finalized after reviews. The team is currently in the active development phase, structured as follows:
* **Phase 1: Environment & Container Setup**: Configure IAM/AWS CLI, build the Docker/Playwright runner (Dockerfile, entrypoint.js, playwright.config.js).
* **Phase 2: Event Pipeline & Coordinator**: Setup SQS + DLQ and develop the Lambda Coordinator calling ECS `RunTask`.
* **Phase 3: Storage & Monitoring**: Provision S3 (frontend and reports), configure CloudWatch log groups and alarms, and create DynamoDB tables for run history and audit logs.
* **Phase 4: AI Summarization**: Develop post-processing Lambda with Secrets Manager integration for OpenAI API keys and circuit-breaker fallbacks.
* **Phase 5: Dashboard & Authorization**: Set up S3 + CloudFront hosting, Cognito user pools, Lambda Authorizers, and implement three role-specific interfaces (Admin / QA-Tester / Developer).
* **Phase 6: Security Hardening**: Configure least-privilege IAM policies, VPC Endpoints, and two scopes of AWS WAF (CloudFront and Regional).
* **Phase 7: Integrated Testing & Demo**: Perform end-to-end testing against a custom-built demo website (to bypass bot protection policies on third-party sites), validate the pipeline, and compile reports.

**Technical Requirements**
* **Test Runner**: Node.js, Playwright, Docker (multi-stage build) to build ECR-destined images.
* **Coordinator Logic**: AWS SDK to call ECS `RunTask` from an SQS-triggered Lambda function.
* **Infrastructure as Code (IaC)**: Recommend provisioning resources using IaC (e.g., AWS CDK/CloudFormation) to ensure environment reproducibility.
* **Security Framework**: Least-privilege IAM roles per component, Secrets Manager for credentials, and VPC Endpoints for internal service queries.

### 5. Roadmap & Implementation Milestones

| Week | Milestone | Responsible |
| ---- | --------- | ----------- |
|      |         |           |

### 6. Budget Estimation

| AWS Service | Core Calculator Configuration | Monthly Cost (USD) |
| ----------- | ----------------------------- | ------------------ |
| **AWS Fargate** | Linux/x86, 50 tasks/day, 1 minute/task, 2 GB RAM, 20 GB ephemeral storage | 1.88 |
| **AWS Lambda** | 10,000 requests/month, 512 MB ephemeral storage | 0.00 |
| **Amazon SQS** | 0.0045 million standard requests/month | 0.00 |
| **Amazon S3 – Frontend** | 1 GB storage, 50 PUTs, 1,500 GETs/month | 0.03 |
| **Amazon S3 – Reports** | 3 GB storage, 37,500 PUTs, 200 GETs/month | 0.26 |
| **Amazon CloudWatch** | 2.2 GB log ingestion, 1 dashboard, 3 standard alarms, 100 API requests | 1.85 |
| **Amazon DynamoDB** | On-Demand, 1 GB storage, average item size 5 KB | 1.88 |
| **Amazon VPC – PrivateLink** | 3 VPC Interface Endpoints/region | 0.05 |
| **AWS Secrets Manager** | 1 secret stored 30 days, 1,500 API calls/month | 0.41 |
| **Amazon Cognito** | 5 MAU, with Advanced Security Features enabled | 0.26 |
| **Amazon CloudFront** | 2,000 HTTPS requests, 1 GB data to origin, 1 GB out to Internet | 0.11 |
| **Amazon API Gateway** | HTTP API, 0.0075 million requests/month, 34 KB/request | 0.01 |
| **Amazon SES** | 4,500 emails sent from Lambda/month | 0.45 |
| **Subtotal (Calculator)** | Services configured on AWS Calculator | **7.19** |
| **NAT Gateway** | Scheduled create/delete to optimize costs, only active during run windows | **15.045** |
| **Total** | Excluding OpenAI API costs | **22.24** |

At **$22.24 USD/month**, the 12-month AWS infrastructure cost is estimated at **$266.82 USD** (excluding third-party OpenAI API charges, which must be added manually based on actual token usage).

> [!IMPORTANT]
> **Key Technical Caveat**: Unlike EC2 instances, NAT Gateways do not support start/stop actions. To achieve the optimized cost of $15.045 USD/month (compared to ~$43 USD/month for 24/7 operation), a scheduled automation workflow using EventBridge Schedule and Lambda must automatically create (`CreateNatGateway`) before execution windows and delete (`DeleteNatGateway`) afterwards. The trade-off is a 1-3 minute delay during NAT initialization, which could introduce latency if a QA tester triggers an on-demand test outside scheduled hours. This trade-off must be highlighted in the risks section of the report.

### 7. Risk Assessment

**Risk Matrix**

| Risk | Impact | Probability |
| ---- | ------ | ----------- |
| ECS Fargate task times out or hangs | Medium | Medium |
| External AI API (OpenAI) unavailable or rate-limited | Low (fallback built-in) | Medium |
| IAM roles assigned excessive permissions during development | High | Medium |
| Backlog in DLQ goes unnoticed without alerting | Medium | Low |
| AWS costs exceed budget due to misconfigured NAT or CloudWatch retention | Medium | Low |
| Latency when QA triggers on-demand tests outside scheduled NAT hours | Medium | Medium |
| Demo website is unstable (if utilizing a live third-party site) | Medium | Medium |

**Mitigation Strategies**
* Configure CloudWatch Alarms for ECS task duration and DLQ message depth to identify stuck tasks or repeated errors.
* Gate the AI step behind a circuit-breaker so the original Pass/Fail reports are still emailed if the AI API fails.
* Enforce least-privilege IAM policies from day one rather than deferring cleanup.
* Set up a DLQ -> CloudWatch Alarm -> SNS alerting pipeline early to avoid silent failures.
* Utilize a dedicated, self-hosted mock website for tests to prevent bot blockades or unpredictable UI changes on third-party domains.
* If a test is triggered manually outside NAT active hours, check NAT status beforehand or accept the 1-3 minute boot latency.

**Contingency Plans**
* If the AI provider is down, fallback to emailing raw HTML/JSON test results.
* If a Fargate task hangs, a CloudWatch alarm will trigger and terminate the task, keeping runs isolated.
* If monthly costs spike, budget alerts will flag anomalies early to adjust log retention or NAT schedules.

### 8. Expected Outcomes
* **Technical Improvements**: Manual E2E checks are replaced by a serverless, event-driven pipeline with no idle infrastructure. Role-based access control (Admin, QA/Tester, Developer) is cleanly enforced at the API border.
* **Long-Term Value**: Provides a reusable event-driven reference architecture for future serverless projects. Aggregated execution history (DynamoDB) forms a foundation for future flaky test analytics. Validates a cost-predictive pay-as-you-go testing model compared to traditional 24/7 environments.