---
title: "Week 12 Worklog"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Week 12 Objectives

* Deploy entire infrastructure and source code to AWS.
* Test the system and complete the report document.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Create detailed deployment plan and configure VPC network infrastructure for the project. | 07/03/2026 | 07/04/2026 |  |
| Saturday | Update and finalize the plan file, prepare source code and configuration files for deployment session. | 07/04/2026 | 07/04/2026 |  |
| Sunday | Phase one deployment: create 2 S3 Buckets, 2 DynamoDB tables and 2 SQS Queues (Task Queue and Dead Letter Queue). | 07/05/2026 | 07/06/2026 | [console.aws.amazon.com (AWS Console)](https://console.aws.amazon.com/) |
| Monday | Deploy 4 Lambda functions, configure EventBridge Scheduler, save API keys in Secrets Manager. Run tests and fix arising configuration errors. | 07/06/2026 | 07/06/2026 | [console.aws.amazon.com (AWS Console)](https://console.aws.amazon.com/) |
| Tuesday | Discovered several critical issues: Lambda missing processing logic, missing DynamoDB table, missing environment variables. Added 2 new DynamoDB tables and partially fixed errors. | 07/07/2026 | 07/09/2026 | [docs.aws.amazon.com (API Gateway CORS)](https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-cors.html) |
| Wednesday | Continue fixing: fixed API Gateway (CORS, missing routes, authorizer, integration), fixed Developer login error, successfully displayed data on website. | 07/08/2026 | 07/09/2026 | [docs.aws.amazon.com (API Gateway CORS)](https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-cors.html) |
| Thursday | Completely fixed manual and automated testing flows. Ran a full system test and got correct results, report email successfully sent. Finished writing deployment report document. | 07/09/2026 | 07/09/2026 | [docs.aws.amazon.com (API Gateway CORS)](https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-cors.html) |

### Week 12 Achievements

* Understood the end-to-end Serverless system deployment process on AWS from network, storage, processing to API.
* Understood the causes and how to handle CORS, authorizer, integration errors in API Gateway.
* Grasped how to debug synchronization errors between Frontend and Backend in distributed systems.
* Understood how EventBridge, SQS, and Lambda coordinate to automatically trigger testing flows.
