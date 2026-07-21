---
title: "Week 3 Worklog"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---
### Week 3 Objectives

* Complete the remaining Labs 10, 19, 20 of Module 02 on Route 53, VPC Peering, and Transit Gateway.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Start Lab 10 on DNS Resolution with Route 53. The CloudFormation template was faulty, so I manually figured out how to configure the Inbound Endpoint and Private Hosted Zone. | 05/01/2026 | 05/02/2026 | [awsstudygroup.com (Lab 10)](https://000010.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Route 53)](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html) |
| Saturday | Continue fixing Lab 10, research more documentation and ask AI for help to complete the DNS Resolution part. | 05/02/2026 | 05/02/2026 | [awsstudygroup.com (Lab 10)](https://000010.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Route 53)](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html) |
| Sunday | Practice Lab 19 on VPC Peering: configure connection between 2 VPCs. Encountered an error where 2 EC2 instances couldn't ping each other, used traceroute to debug the Route Table. | 05/03/2026 | 05/04/2026 | [awsstudygroup.com (Lab 19)](https://000019.awsstudygroup.com/vi/) - [docs.aws.amazon.com (VPC Peering)](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html) |
| Monday | Continue fixing Lab 19 error: corrected the Route Table direction and successfully pinged. | 05/04/2026 | 05/04/2026 | [awsstudygroup.com (Lab 19)](https://000019.awsstudygroup.com/vi/) - [docs.aws.amazon.com (VPC Peering)](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html) |
| Tuesday | Start Lab 20: create Transit Gateway to act as a central hub connecting multiple VPCs instead of VPC Peering. | 05/05/2026 | 05/07/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Transit Gateway)](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html) |
| Wednesday | Continue Lab 20: configure Route Table for Transit Gateway so the VPCs can communicate with each other. | 05/06/2026 | 05/07/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EFS)](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) - [docs.aws.amazon.com (Amazon FSx)](https://docs.aws.amazon.com/fsx/) |
| Thursday | Complete Lab 20: run tests and confirm EC2-01 can ping EC2-02, EC2-03, EC2-04 via internal network. | 05/07/2026 | 05/07/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Transit Gateway)](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html) |

### Week 3 Achievements

* Understood the DNS Resolution mechanism with Route 53 and how to manually configure Inbound Endpoint and Private Hosted Zone when CloudFormation fails.
* Understood how VPC Peering works and the role of the Route Table in routing traffic between VPCs.
* Understood what Transit Gateway is and why it's more suitable than VPC Peering when connecting multiple VPCs simultaneously.
