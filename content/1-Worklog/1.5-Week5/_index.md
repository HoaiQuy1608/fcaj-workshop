---
title: "Week 5 Worklog"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives:

* Study Module 05 on security (IAM, KMS, Lambda, CloudWatch) and Module 06 on databases.
* Practice security and system monitoring labs.

### Tasks to be carried out this week:
| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Watch videos on AWS security services of Module 05. Due to access denial to Security Hub, read Lab 18 documentation only. Practice Lab 22 on automated start/stop of EC2 using Lambda: created EC2, assigned tags, wrote Lambda start/stop function, configured EventBridge Scheduler, and set up Slack notifications. Resolved an EC2 tag issue, after setting the tag environment_auto=true and retesting Lambda code, the system worked correctly, successfully sent notifications to Slack, and start/stop EC2 ran normally. | 05/15/2026 | 05/15/2026 | [youtube.com](https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150) - [youtube.com](https://www.youtube.com/watch?v=esPRIj_zZSQ&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=161) - [awsstudygroup.com (Lab 22)](https://000022.awsstudygroup.com/vi/) |
| Saturday | Practice Lab 28 on EC2 access management using Resource Tags via IAM. Created IAM Users and Roles, and configured IAM Policies to control permissions to view, tag, launch, and manage EC2 based on Region and Tags. Checked access rights and tested successful/denied cases when Region or Tags were incorrect to understand IAM Condition using aws:RequestedRegion, aws:RequestTag, and ec2:ResourceTag. | 05/16/2026 | 05/16/2026 | [awsstudygroup.com (Lab 28)](https://000028.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=vkBJ0Cxc6Nw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=177) |
| Sunday | Practice Lab 30 on IAM Permission Boundary. Created an IAM Policy restricting EC2 access by Region, created an IAM User, and assigned AmazonEC2FullAccess combined with Permission Boundary. Tested user access inside allowed Regions and verified blocked access outside the boundary to understand how Permission Boundary limits maximum user permissions even with a broad policy. | 05/17/2026 | 05/17/2026 | [youtube.com](https://www.youtube.com/watch?v=rZ2oeD0Ok5U&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=188) - [awsstudygroup.com (Lab 30)](https://000030.awsstudygroup.com/vi/) |
| Monday | Practice Lab 33 on encrypting S3 data at rest with AWS KMS. Created KMS Key, configured S3 object encryption using the key, and tested access permissions. Verified that users without KMS key permissions could not read objects even if S3 access was permitted, demonstrating KMS as an extra access control layer. <br> Practice Lab 44 on IAM Roles and IAM Conditions. Created IAM User, Group, and Role to test switch role mechanism. Configured trust policy for the role to restrict assume role by source IP using aws:SourceIp and time using aws:CurrentTime. Resolved switch role session cache issue by logging in using a different browser. | 05/18/2026 | 05/18/2026 | [youtube.com](https://www.youtube.com/watch?v=XPUfX9proJg&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=191) - [awsstudygroup.com (Lab 33)](https://000033.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=ptog1aBHeko&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=202) - [awsstudygroup.com (Lab 44)](https://000044.awsstudygroup.com/vi/) |
| Tuesday | Practice Lab 48 on configuring IAM Roles for EC2 to access S3 securely. Tested two methods: using Access/Secret Keys of an IAM User, and using an IAM Role attached directly to EC2. Understood security risks of hardcoding Access Keys and migrated to using IAM Roles for EC2 instances. | 05/19/2026 | 05/19/2026 | [youtube.com](https://www.youtube.com/watch?v=jk4dr_DYxWs&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=210) - [awsstudygroup.com (Lab 48)](https://000048.awsstudygroup.com/vi/) |
| Wednesday | Practice Lab 08 (Module 03) on Amazon CloudWatch. Redeployed environment with CloudFormation, observed Metrics, Logs, Logs Insights, Metric Filters, Alarms, and Dashboards. Resolved an issue where logger.py script was missing in S3 by writing a python script to simulate logs on EC2 for CloudWatch Agent to push metrics/logs to CloudWatch. | 05/20/2026 | 05/20/2026 | [awsstudygroup.com (Lab 8)](https://000008.awsstudygroup.com/vi/) |
| Thursday | Watch video lectures of Module 06 on AWS RDS and Aurora, and read documentation to study database services. | 05/21/2026 | 05/22/2026 | [youtube.com](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) - [docs.aws.amazon.com](https://docs.aws.amazon.com/rds/) |

### Week 5 Achievements:

* Completed hands-on labs related to security (IAM Policies, IAM Roles, Permission Boundaries, and IAM Conditions) for fine-grained access control.
* Understood the security risks of direct Access Key usage and migrated to using IAM Roles for EC2 instances for better security.
* Successfully implemented automated start/stop EC2 scripts via Lambda combined with EventBridge Scheduler and Slack notifications.
* Configured S3 data encryption using AWS KMS and managed KMS Key permissions.
* Gained experience in monitoring systems using Amazon CloudWatch (CloudWatch Agent, Metrics, Logs, Alarms, and Dashboards).
