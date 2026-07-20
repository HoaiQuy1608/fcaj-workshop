---
title: "Week 12 Worklog"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Week 12 Objectives

* Plan, configure network infrastructure, and prepare necessary resources for the project.
* Deploy services and conduct system trial tests.
* Document the entire deployment process into the project report.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | - Create a deployment plan and configure the VPC network infrastructure. | 07/03/2026 | 07/03/2026 |  |
| Saturday | - Update and finalize the deployment plan and prepare assets (source code, configuration files). | 07/04/2026 | 07/04/2026 |  |
| Sunday | - Deploy the phase of the project: configure storage and database resources including 2 S3 buckets, 2 DynamoDB tables, and 2 SQS queues (task queue and Dead Letter Queue). | 07/05/2026 | 07/05/2026 |  |
| Monday | - Continue infrastructure deployment: create and configure 4 Lambda functions, set up EventBridge Scheduler triggers, securely store API keys in AWS Secrets Manager; fix configuration bugs and run system trial tests. | 07/06/2026 | 07/06/2026 |  |
| Tuesday | - Ran a trial test of the website and discovered multiple issues: frontend and backend out of sync due to Lambda functions missing logic to persist data, missing DynamoDB tables, and missing environment variables. Partially resolved by adding 2 DynamoDB tables. | 07/07/2026 | 09/07/2026 |  |
| Wednesday | - Continued resolving issues: fixed create test suite feature and dropdown. Resolved API Gateway CORS blocking, missing routes and authorizers. Fixed Developer login bug. | 07/08/2026 | 07/09/2026 |  |
| Thursday | - Quickly resolved a data display bug on the website, addressed all remaining issues. The system ran successfully. | 07/09/2026 | 07/09/2026 |  |

### Week 12 Achievements

* Aligned on a detailed deployment plan and successfully configured the VPC network infrastructure.
* Provisioned and configured storage, database, and message queue services: 2 S3 buckets, 2 DynamoDB tables, and 2 SQS queues (including Dead Letter Queue).
* Deployed and configured 4 Lambda functions, set up EventBridge Scheduler triggers, and securely stored API keys using AWS Secrets Manager.
* Identified and resolved multiple critical issues during trial testing: frontend/backend mismatch, missing Lambda logic, missing DynamoDB tables, misconfigured API Gateway, and missing environment variables.
* Fixed all debug issues: resolved CORS, added missing routes, authorizers, and integrations to API Gateway, fixed a Developer login bug, and added missing tables and environment variables.
* Successfully ran the full system test flow (manual and automated), confirmed correct execution results and successful delivery of report emails. Completed the deployment report.
