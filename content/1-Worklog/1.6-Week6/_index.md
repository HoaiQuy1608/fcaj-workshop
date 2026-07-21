---
title: "Week 6 Worklog"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Week 6 Objectives

* Learn about AWS RDS & Aurora services, practice Lab 05, Lab 06, and remaining missing labs.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Read more documentation on RDS, Aurora and re-watch Module 06 video lectures to review theory before practicing. | 05/22/2026 | 05/22/2026 | [docs.aws.amazon.com (Amazon RDS)](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) - [docs.aws.amazon.com (Amazon Aurora)](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html) |
| Saturday | Practice Lab 05 on Amazon RDS: create RDS MySQL, install Node.js + MySQL client on EC2, deploy app connecting to RDS. Encountered error where mysql package was incompatible with MySQL 8.4, fixed by switching to mysql2. | 05/23/2026 | 05/23/2026 | [awsstudygroup.com (Lab 5)](https://000005.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon RDS)](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) |
| Sunday | Review SQL from basic to advanced: SELECT, JOIN, GROUP BY, subqueries. | 05/24/2026 | 05/24/2026 | [w3schools.com (SQL)](https://www.w3schools.com/sql/) |
| Monday | Practice Lab 06 on Auto Scaling Group and Elastic Load Balancing. Fixed 502 Bad Gateway error by checking health check and port 5000 in Security Group. | 05/25/2026 | 05/25/2026 | [awsstudygroup.com (Lab 6)](https://000006.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon DynamoDB)](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html) |
| Tuesday | Practice Lab 45 on Amazon Lightsail: deploy WordPress + Lightsail Database, configure networking and firewall. A few final steps failed so only read documentation. | 05/26/2026 | 05/26/2026 | [awsstudygroup.com (Lab 45)](https://000045.awsstudygroup.com/vi/) |
| Wednesday | Learn the overall architecture of Lab 35 on Data Lake (S3, Kinesis, Glue, Athena, QuickSight). Account was limited for Kinesis and Glue Crawler so only read documentation on the operational flow. | 05/27/2026 | 05/27/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) |
| Thursday | Practice Lab 60 on DynamoDB: create tables, perform CRUD operations, Global Secondary Index using AWS CLI and Python SDK boto3. | 05/28/2026 | 05/28/2026 | [awsstudygroup.com (Lab 60)](https://000060.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Lightsail)](https://docs.aws.amazon.com/lightsail/) |

### Week 6 Achievements

* Understood how RDS MySQL works and how a Node.js application connects to RDS through a Security Group.
* Understood the mechanism of Auto Scaling Group and Load Balancer coordinating to balance load and automatically scale the system.
* Grasped how to operate DynamoDB using AWS CLI and Python SDK (boto3) and the difference between Query and Scan.
* Understood the overall Data Lake architecture and the role of each service in the data analytics pipeline.
