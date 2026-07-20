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
| Friday | Review Module 06 and read documentation on Amazon RDS and Aurora services. | 05/22/2026 | 05/22/2026 | [youtube.com](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) - [docs.aws.amazon.com](https://docs.aws.amazon.com/rds/) |
| Saturday | Practice Lab 05 on Amazon RDS. Created RDS MySQL database, configured Security Group for EC2 to connect to RDS, installed Node.js and MySQL client on EC2, created database/table, and deployed a Node.js application connecting to RDS. During execution, encountered an error due to an empty .env file and the mysql package being incompatible with MySQL 8.4; fixed by reconfiguring .env and switching to mysql2. Finally, the application ran successfully on port 5000 and successfully connected to RDS. | 05/23/2026 | 05/23/2026 | [awsstudygroup.com (Lab 5)](https://000005.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=B5rOeWQWg1c&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=220) |
| Sunday | Review SQL queries from basic to advanced. | 05/24/2026 | 05/24/2026 | |
| Monday | Practice Lab 06 on Auto Scaling Group and Elastic Load Balancing. Deployed web application on EC2, configured RDS database, created Launch Template, Target Group, Application Load Balancer, and Auto Scaling Group. During testing, resolved a 502 Bad Gateway error by verifying health check settings, port 5000, and Security Groups until the target status turned healthy. | 05/25/2026 | 05/25/2026 | [awsstudygroup.com (Lab 6)](https://000006.awsstudygroup.com/vi/) |
| Tuesday | Practice Lab 45 (Module 03) on Amazon Lightsail. Created Lightsail Database and deployed WordPress instance, configured WordPress database connection via DB_HOST, DB_USER, DB_PASSWORD, and DB_NAME. During implementation, resolved database connection errors caused by incorrect endpoint or database name. Explored and configured Lightsail networking/firewall, verified SSH/HTTP/HTTPS rules, and practiced application security. The remaining 2 instances failed at some steps so they were stopped; read documentation on creating snapshots, upgrading to larger instances, and setting up alarms instead. | 05/26/2026 | 05/26/2026 | [awsstudygroup.com (Lab 45)](https://000045.awsstudygroup.com/vi/) |
| Wednesday | Study Lab 35 (Module 07) on Data Lake on AWS. Read the overall architecture of the data pipeline consisting of S3, Kinesis Data Firehose, AWS Glue Data Catalog, Glue Crawler, Athena, and QuickSight. During practice, the AWS account had restricted access to Kinesis Data Firehose and AWS Glue Crawler, preventing the creation of Delivery Streams, running CloudFormation related to Kinesis, or creating crawlers to catalog data. Therefore, switched to reading and understanding the Data Lake workflow and the role of each service. | 05/27/2026 | 05/27/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=uYCW51_pBBA&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=246) |
| Thursday | Practice Lab 60 on Amazon DynamoDB. Created DynamoDB tables using AWS CLI, performed CRUD operations, queried data via Query/Scan, and created and queried Global Secondary Indexes. Then used Python SDK Boto3 to execute table creation, update, deletion, read, loading sample data, querying, and item deletion. | 05/28/2026 | 05/28/2026 | [awsstudygroup.com (Lab 60)](https://000060.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=cqczgtnvHjc&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=273) |

### Week 6 Achievements

* Gained a deeper understanding of databases on AWS including Amazon RDS, DynamoDB, Lightsail Database, and co-scaling mechanisms (Auto Scaling / Elastic Load Balancing).
* Successfully deployed a Node.js application connected to RDS MySQL and resolved database package version issues.
* Successfully configured Auto Scaling Group with Application Load Balancer for automatic scaling and routing, resolving 502 Bad Gateway errors through health checks.
* Practiced table creation, CRUD operations, and Global Secondary Index (GSI) configurations on DynamoDB using AWS CLI and Python SDK (Boto3).
* Deployed WordPress and database on Amazon Lightsail and understood networking/firewall setups in Lightsail.
* Mastered Data Lake architecture flows and the roles of Kinesis, S3, Glue, and Athena.
