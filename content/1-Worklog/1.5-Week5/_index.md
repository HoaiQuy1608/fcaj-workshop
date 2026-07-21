---
title: "Week 5 Worklog"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives

* Learn Module 05 on AWS Security (IAM, KMS, Lambda, CloudWatch).
* Practice various security and system monitoring labs.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Watch Module 05 video on AWS security. Practice Lab 22: write Lambda to auto start/stop EC2 by tag, configure EventBridge Scheduler, send Slack notifications. | 05/15/2026 | 05/15/2026 | [awsstudygroup.com (Lab 22)](https://000022.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Auto Scaling)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html) - [docs.aws.amazon.com (ELB)](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html) |
| Saturday | Practice Lab 28: create IAM User/Role with IAM Policy to control EC2 access by Region and Tag, test allowed and denied cases to understand IAM Condition. | 05/16/2026 | 05/16/2026 | [awsstudygroup.com (Lab 28)](https://000028.awsstudygroup.com/vi/) - [docs.aws.amazon.com (IAM Policies)](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html) |
| Sunday | Practice Lab 30: configure Permission Boundary to limit the maximum permissions of an IAM User despite broad attached policies. | 05/17/2026 | 05/17/2026 | [awsstudygroup.com (Lab 30)](https://000030.awsstudygroup.com/vi/) - [docs.aws.amazon.com (IAM Policies)](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html) |
| Monday | Practice Lab 33: encrypt S3 objects using AWS KMS, set permissions for KMS Key. Practice Lab 44: create Trust Policy to limit access by source IP and time. | 05/18/2026 | 05/18/2026 | [awsstudygroup.com (Lab 33)](https://000033.awsstudygroup.com/vi/) - [awsstudygroup.com (Lab 44)](https://000044.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS KMS)](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html) |
| Tuesday | Practice Lab 48: compare 2 ways to grant EC2 access to S3 (Access Key vs. IAM Role), understand security risks when hardcoding credentials. | 05/19/2026 | 05/19/2026 | [awsstudygroup.com (Lab 48)](https://000048.awsstudygroup.com/vi/) |
| Wednesday | Practice Lab 08 on CloudWatch: deploy environment using CloudFormation, write Python script to simulate logs on EC2 (original logger.py file missing on S3), set up Metrics, Alarms, Dashboards. | 05/20/2026 | 05/20/2026 | [awsstudygroup.com (Lab 8)](https://000008.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon CloudWatch)](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| Thursday | Watch Module 06 video on AWS RDS and Aurora, read documentation to prepare for next week. | 05/21/2026 | 05/21/2026 | [docs.aws.amazon.com (Amazon RDS)](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) - [docs.aws.amazon.com (Amazon Aurora)](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html) |

### Week 5 Achievements

* Understood how IAM Policy, IAM Condition, and Permission Boundary work to control detailed access rights.
* Understood the security risks of using Access Keys and why attaching an IAM Role to EC2 is the correct approach.
* Understood how KMS encrypts S3 data and acts as an additional access control layer.
* Grasped how CloudWatch collects metrics/logs from EC2 and how to configure Alarms and Dashboards for system monitoring.
