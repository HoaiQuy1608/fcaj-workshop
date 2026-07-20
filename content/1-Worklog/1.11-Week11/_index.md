---
title: "Week 11 Worklog"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Week 11 Objectives

* Finalize the optimized, cost-efficient, and secure architecture diagram for the group project.
* Distribute tasks among team members and prepare the deployment environment.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | - Hold a group meeting to optimize the architecture diagram: decided to remove the SNS service as it was unnecessary for the group project, replaced AWS Bedrock with another solution due to Free Tier account restrictions, and discussed VPC network configuration options. | 06/26/2026 | 06/26/2026 |  |
| Saturday | - Continue refining the architecture with the team: adjusted the SQS message queue trigger for Lambda, and reviewed and configured system monitoring with CloudWatch. | 06/27/2026 | 06/27/2026 |  |
| Sunday | - Configure detailed data flows on the architecture diagram, focusing on resolving the network subnets for Lambda Processing within the VPC. | 06/28/2026 | 06/28/2026 |  |
| Monday | - Group related resources on the architecture diagram to increase visual clarity. | 06/29/2026 | 06/29/2026 |  |
| Tuesday | - Continue modifying the architecture with the team: placed Lambda Processing inside Private Subnets routing via NAT Gateway and VPC Endpoints to communicate with external AI; completed the final architecture diagram. | 06/30/2026 | 06/30/2026 |  |
| Wednesday | - Distribute specific tasks to team members and finalized the technology stack (Next.js for Frontend and Python Boto3 for Backend). | 07/01/2026 | 07/01/2026 |  |
| Thursday | -  | 07/02/2026 | 07/02/2026 |  |

### Week 11 Achievements

* Finalized the optimized and secure system architecture: placed ECS Fargate in Private Subnets with VPC Endpoints for secure local communication with S3, DynamoDB, and ECR; placed the processing Lambda inside Private Subnets routing via NAT Gateway to access the ChatGPT API.
* Distributed specific tasks to team members and finalized the technology stack (Next.js for Frontend, Python Boto3 SDK for Backend).
* Prepared the deployment environment: created IAM accounts, scheduled deployment phases, and prepared data schemas as well as VPC network configurations.
