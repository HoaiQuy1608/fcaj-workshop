---
title: "Week 12 Worklog"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Week 12 Objectives:

* Plan, configure network infrastructure, and prepare necessary resources for the project.
* Deploy services and conduct system trial tests.
* Document the entire deployment process into the project report.

### Tasks to be carried out this week:
| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Create a deployment plan and configure the VPC network infrastructure. | 07/03/2026 | 07/03/2026 |  |
| Saturday | Update and finalize the deployment plan and prepare assets (source code, configuration files). | 07/04/2026 | 07/04/2026 |  |
| Sunday | Deploy the initial phase of the project: configure storage and database resources including 2 S3 buckets, 2 DynamoDB tables, and 2 SQS queues (task queue and Dead Letter Queue). | 07/05/2026 | 07/05/2026 |  |
| Monday | Continue infrastructure deployment: create and configure 4 Lambda functions, set up EventBridge Scheduler triggers, securely store API keys in AWS Secrets Manager; fix configuration bugs and run system trial tests. | 07/06/2026 | 07/06/2026 |  |
| Tuesday | Ran a trial test of the website and discovered multiple critical issues: frontend and backend were out of sync due to Lambda functions missing the logic to persist data to DynamoDB and S3, missing handlers for several features, missing DynamoDB tables for test suites and email config, and missing environment variables required by the Lambda functions. Partially resolved: added 2 DynamoDB tables for test history and email config; however, the remaining features and data display on the website were not yet addressed. | 07/07/2026 | 07/09/2026 |  |
| Wednesday | Continued resolving issues carried over from Tuesday: fixed the create test suite feature and its persistence to the database, fixed the test suite dropdown in the manual trigger section. Discovered additional issues: API Gateway blocked by CORS, routes missing for several features, authorizers and integrations not fully configured, and missing trigger connecting to the Lambda backend for UI rendering. Resolved all API Gateway issues, added the automated test schedule feature, fixed a Developer login bug in the source code, and successfully displayed data on the website. The manual and automated test execution flows were still not fully functional. | 07/08/2026 | 07/09/2026 |  |
| Thursday | Quickly resolved a data display bug on the website, then addressed all remaining issues from the previous two days. Focused on fixing the core test execution flow (both manual and automated) and completed it within the day. Successfully ran a full website test — the system returned results and sent the report email as expected. Finished writing up all deployment activities in the project report. | 07/09/2026 | 07/09/2026 |  |

### Week 12 Achievements:

* Aligned on a detailed deployment plan and successfully configured the VPC network infrastructure.
* Provisioned and configured storage, database, and message queue services: 2 S3 buckets, 2 DynamoDB tables, and 2 SQS queues (including Dead Letter Queue).
* Deployed and configured 4 Lambda functions, set up EventBridge Scheduler triggers, and securely stored API keys using AWS Secrets Manager.
* Identified and resolved multiple critical issues during trial testing: frontend/backend mismatch, missing Lambda logic, missing DynamoDB tables, misconfigured API Gateway, and missing environment variables.
* Fixed all debug issues: resolved CORS, added missing routes, authorizers, and integrations to API Gateway, fixed a Developer login bug, and added missing tables and environment variables.
* Successfully ran the full system test flow (manual and automated), confirmed correct execution results and successful delivery of report emails. Completed the deployment report.
