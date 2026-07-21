---
title: "Week 10 Worklog"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Week 10 Objectives

* Complete project description and draw detailed architecture diagram.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Continue and complete detailed project description: overall operational flow, analyze each AWS service to be used. | 06/19/2026 | 06/19/2026 | |
| Saturday | Start drawing architecture diagram: define AWS services and positions in each layer (Frontend, Backend, Database, Networking). | 06/20/2026 | 06/25/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Sunday | Connect data flows between CloudFront, API Gateway, Lambda, SQS, ECS, DynamoDB on the diagram. | 06/21/2026 | 06/25/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Monday | Add security layer to the diagram (Cognito, IAM Role, Security Group, VPC) and review all flows. | 06/22/2026 | 06/25/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Tuesday | Finalize the diagram and post it on the group for admins to review. Received feedback with quite a few configuration errors, group met to discuss fixes. | 06/23/2026 | 06/25/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Wednesday | Group meeting to absorb feedback and adjust incorrect connection flows in the diagram. | 06/24/2026 | 06/25/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Thursday | Fix errors based on feedback: successfully fixed connection flow from User to CloudFront, S3 and Internet Gateway. | 06/25/2026 | 06/25/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |

### Week 10 Achievements

* Completed detailed project description with full operational flow and AWS service analysis.
* Better understood common architectural design flaws after receiving feedback from admins.
* Grasped how data flows from the user side through CloudFront, S3 to backend services.
