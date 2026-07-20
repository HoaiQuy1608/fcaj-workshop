---
title: "Week 5 Worklog"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives

* Study Module 05 on security (IAM, KMS, Lambda, CloudWatch) and Module 06 on databases.
* Practice security and system monitoring labs.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | - Start Module 05 on AWS Security.<br>- Practice Lab 22: Auto start/stop EC2 using Lambda.<br>- Fix EC2 tag mismatch, update to `environment_auto=true` and the Lambda function runs successfully. | 05/15/2026 | 05/15/2026 | |
| Saturday | - Practice Lab 28: Manage EC2 access with Resource Tags via IAM.<br>- Configure IAM Conditions to limit server start/stop permissions according to project tags. | 05/16/2026 | 05/16/2026 | |
| Sunday | - Practice Lab 30 on IAM Permission Boundary.<br>- Apply policy boundary to restrict maximum user permissions within the allowed Region. | 05/17/2026 | 05/17/2026 | |
| Monday | - Practice Lab 33: Encrypt S3 data using AWS KMS.<br>- Practice Lab 44: Configure Trust Policy for IAM Role.<br>- Resolve browser session cache issue when testing switch role. | 05/18/2026 | 05/18/2026 | |
| Tuesday | - Practice Lab 48: Grant EC2 access to S3.<br>- Directly compare security risks between using IAM Roles and hardcoding Access Keys. | 05/19/2026 | 05/19/2026 | |
| Wednesday | - Practice Lab 08 (Module 03) on Amazon CloudWatch.<br>- The `logger.py` file is missing on S3, write a custom Python script to mock sending logs from EC2 to CloudWatch Log Group. | 05/20/2026 | 05/20/2026 | |
| Thursday | - Watch Module 06 lecture videos on Amazon RDS and Aurora.<br>- Read documentation on Multi-AZ architecture and Read Replicas in preparation for tomorrow's lab. | 05/21/2026 | 05/21/2026 | |

### Week 5 Achievements

* Completed hands-on labs related to security (IAM Policies, IAM Roles, Permission Boundaries, and IAM Conditions) for fine-grained access control.
* Understood the security risks of direct Access Key usage and migrated to using IAM Roles for EC2 instances for better security.
* Successfully implemented automated start/stop EC2 scripts via Lambda combined with EventBridge Scheduler and Slack notifications.
* Configured S3 data encryption using AWS KMS and managed KMS Key permissions.
* Gained experience in monitoring systems using Amazon CloudWatch (CloudWatch Agent, Metrics, Logs, Alarms, and Dashboards).
