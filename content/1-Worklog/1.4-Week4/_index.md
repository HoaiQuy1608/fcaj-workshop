---
title: "Week 4 Worklog"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Week 4 Objectives

* Learn theory of Module 03, Module 04 on EC2 and Storage.
* Practice Lab 13, Lab 57, Lab 58, Lab 04, and Lab 27.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Watch video lectures for Module 03 and Module 04 on EC2 servers, S3, EBS, and EFS. | 05/08/2026 | 05/08/2026 | [docs.aws.amazon.com (Amazon EC2)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) - [docs.aws.amazon.com (Amazon S3)](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) |
| Saturday | Start Lab 13 on AWS Backup automation: run CloudFormation to create environment, set up basic Backup Vault and Backup Plan. | 05/09/2026 | 05/10/2026 | [awsstudygroup.com (Lab 13)](https://000013.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS Backup)](https://docs.aws.amazon.com/aws-backup/latest/devguide/whatisbackup.html) |
| Sunday | Complete Lab 13: configure SNS for notifications and write Lambda to handle automated backup events. Practice Lab 57: create S3 Bucket for static website hosting, only read documentation for CloudFront due to account limitations. | 05/10/2026 | 05/10/2026 | [awsstudygroup.com (Lab 57)](https://000057.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon CloudFront)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| Monday | Read review materials on IAM Role, VPC Endpoints, and Session Manager to prepare for Lab 58. | 05/11/2026 | 05/13/2026 | [docs.aws.amazon.com](https://docs.aws.amazon.com) |
| Tuesday | Start Lab 58 (Session Manager): create IAM Role, initialize Public Linux EC2 and Private Windows EC2. | 05/12/2026 | 05/13/2026 | [awsstudygroup.com (Lab 58)](https://000058.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS Systems Manager)](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html) |
| Wednesday | Continue Lab 58: configure VPC Endpoints. The Windows EC2 didn't show up in Managed Nodes, found out it was due to missing HTTPS 443 rule in Security Group, added it and connected successfully. | 05/13/2026 | 05/13/2026 | [awsstudygroup.com (Lab 58)](https://000058.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS Systems Manager)](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html) |
| Thursday | Practice Lab 27 (tagging resources) and Lab 04 (creating Windows/Linux EC2, Snapshot, Custom AMI). | 05/14/2026 | 05/14/2026 | [awsstudygroup.com (Lab 27)](https://000027.awsstudygroup.com/vi/) - [awsstudygroup.com (Lab 4)](https://000004.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EC2)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) |

### Week 4 Achievements

* Understood the AWS Backup automation process combining CloudFormation, SNS, and Lambda.
* Understood how Session Manager works and why VPC Endpoints are necessary to connect to private EC2 without a public IP.
* Grasped how S3 is used to host static websites and the role of CloudFront in content distribution.
* Understood how Tags and Resource Groups help categorize and manage AWS resources effectively.
