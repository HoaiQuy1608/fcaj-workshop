---
title: "Week 11 Worklog"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Week 11 Objectives

* Optimize architecture for security and cost.
* Unify the technology stack and start preparing for deployment.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Group meeting to optimize diagram: removed SNS as unnecessary, replaced Bedrock with another solution due to Free Tier limitations. | 06/26/2026 | 06/30/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Saturday | Continue adjusting architecture: adjust SQS flow triggering Lambda and configure CloudWatch monitoring. | 06/27/2026 | 06/30/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Sunday | Configure network segmentation: put Lambda Processing in Private Subnet, use NAT Gateway to call external APIs and VPC Endpoints for internal communication with S3, DynamoDB, ECR. | 06/28/2026 | 06/30/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Monday | Add Cognito to architecture for user authorization, group related resources on the diagram for clarity. | 06/29/2026 | 06/30/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Tuesday | Finalize the ultimate architecture diagram, assign specific tasks to each member and unify stack: Frontend Next.js, Backend Python Boto3. | 06/30/2026 | 06/30/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Wednesday | Start writing Backend source code: setup Python project, write API functions and configure connections to AWS services. | 07/01/2026 | 07/02/2026 | [boto3.amazonaws.com (Boto3 Docs)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) |
| Thursday | Initialize IAM accounts for each member, create detailed deployment plan and prepare DynamoDB schema file and VPC configuration for deployment week. | 07/02/2026 | 07/02/2026 | [boto3.amazonaws.com (Boto3 Docs)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) |

### Week 11 Achievements

* Understood why Lambda needs to be placed in a Private Subnet and use NAT Gateway instead of exposing Lambda directly to the Internet.
* Understood the role of VPC Endpoints in helping resources in Private Subnets communicate with S3, DynamoDB without going through the Internet.
* Grasped the reason for choosing Next.js for Frontend and Python Boto3 for Backend in the context of the project.
