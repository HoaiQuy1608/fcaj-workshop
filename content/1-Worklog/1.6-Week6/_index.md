---
title: "Week 6 Worklog"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Week 6 Objectives

* Learn about AWS RDS & Aurora services, complete related labs, and catch up on remaining labs.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | - Review Module 06 lecture videos.<br>- Read technical documentation on the architecture and features of Amazon RDS & Aurora services. | 05/22/2026 | 05/22/2026 | |
| Saturday | - Practice Lab 05 on Amazon RDS.<br>- Encounter an empty `.env` file and mysql package incompatibility with MySQL 8.4 authentication.<br>- Reconfigure and switch to the `mysql2` library to connect successfully. | 05/23/2026 | 05/23/2026 | |
| Sunday | - Spend time reviewing SQL syntax.<br>- Test basic data retrieval and table join queries on the newly created RDS instance. | 05/24/2026 | 05/24/2026 | |
| Monday | - Practice Lab 06 (Module 03) on Auto Scaling Group (ASG) and Elastic Load Balancing (ELB).<br>- Encounter 502 Bad Gateway error due to Health Check failure.<br>- Check port 5000 and Security Group, adjust to make the Target Group healthy. | 05/25/2026 | 05/25/2026 | |
| Tuesday | - Practice Lab 45 (Module 03) on Amazon Lightsail.<br>- Fix application database connection error caused by incorrect endpoint and DB name. | 05/26/2026 | 05/26/2026 | |
| Wednesday | - Practice Lab 60 on Amazon DynamoDB.<br>- Use AWS CLI and Python SDK (boto3) to execute CRUD commands and create a Global Secondary Index (GSI). | 05/27/2026 | 05/27/2026 | |
| Thursday | - Start reading documentation for Lab 35 (Module 07) on Data Lake.<br>- Due to lab account restrictions on creating Kinesis Data Firehose, only read documentation to understand the data flow. | 05/28/2026 | 05/28/2026 | |

### Week 6 Achievements

* Gained a deeper understanding of databases on AWS including Amazon RDS, DynamoDB, Lightsail Database, and co-scaling mechanisms (Auto Scaling / Elastic Load Balancing).
* Successfully deployed a Node.js application connected to RDS MySQL and resolved database package version issues.
* Successfully configured Auto Scaling Group with Application Load Balancer for automatic scaling and routing, resolving 502 Bad Gateway errors through health checks.
* Practiced table creation, CRUD operations, and Global Secondary Index (GSI) configurations on DynamoDB using AWS CLI and Python SDK (Boto3).
* Deployed WordPress and database on Amazon Lightsail and understood networking/firewall setups in Lightsail.
* Mastered Data Lake architecture flows and the roles of Kinesis, S3, Glue, and Athena.
