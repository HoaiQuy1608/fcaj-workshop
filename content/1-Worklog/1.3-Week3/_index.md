---
title: "Week 3 Worklog"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---
### Week 3 Objectives

* Practice and complete Labs 10, 19, and 20 of Module 02.
* Learn the basic theoretical content of Module 03.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | - Watch the video and read the documentation for Lab 19 of Module 02. | 05/01/2026 | 05/01/2026 | [youtube.com](https://www.youtube.com/watch?v=sllYqAECBoM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=56) |
| Saturday | - Watch the video and read the documentation for Lab 20 of Module 02. | 05/02/2026 | 05/02/2026 | [youtube.com](https://www.youtube.com/watch?v=sllYqAECBoM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=566) |
| Sunday | - Review the videos and read the documentation for Labs 10, 19, and 20 to prepare for practice. | 05/03/2026 | 05/03/2026 |  |
| Monday | - Practice Lab 10. <br> - Since the sample CloudFormation template failed to deploy, researched and manually configured the Inbound Endpoint and Private Hosted Zone to complete DNS Resolution. | 05/04/2026 | 05/04/2026 | [awsstudygroup.com (Lab 10)](https://000010.awsstudygroup.com/vi/) |
| Tuesday | - Continue practicing and complete Lab 10. <br> - read further documentations and researched with AI Chat to deploy it successfully. | 05/05/2026 | 05/05/2026 | [awsstudygroup.com (Lab 10)](https://000010.awsstudygroup.com/vi/) |
| Wednesday | - Practice Lab 19 on VPC Peering. <br> - Encountered an issue where two EC2 instances could not ping each other. <br> - used the traceroute tool to detect routing errors and completed the lab. <br> - Continue to explore Lab 20. | 05/06/2026 | 05/06/2026 | [awsstudygroup.com (Lab 19)](https://000019.awsstudygroup.com/vi/) |
| Thursday | - Practice Lab 20. <br> - Created a Transit Gateway and configured Route Tables to manage connections and allow EC2-01 to successfully ping EC2-02, EC2-03, and EC2-04. | 05/07/2026 | 05/07/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) |

### Week 3 Achievements

* Completed hands-on practices for Lab 10, Lab 19, and Lab 20 of Module 02.
* Configured Inbound Endpoint and Private Hosted Zone manually to resolve DNS Resolution issues when the CloudFormation template failed.
* Implemented VPC Peering to connect isolated VPC networks.
* Deployed Transit Gateway to optimize traffic routing between multiple VPCs.
| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |\n| :---: | :--- | :---: | :---: | :--- |\n| Friday | - Start practicing Lab 19 on VPC Peering. Initialize the environment using CloudFormation and configure Peering. Read documentation while working. Delete the stack at the end of the day to avoid billing. | 05/01/2026 | 05/01/2026 | |\n| Saturday | - Recreate Lab 19 environment. Configure Route Tables but encountered an issue where 2 EC2 instances couldn't ping each other. Learned how to use the traceroute tool to analyze network flow. Delete stack at the end of the day. | 05/02/2026 | 05/02/2026 | |\n| Sunday | - Recreate Lab 19 environment. Apply traceroute to detect routing errors, update the Route Table, and successfully ping. Complete the lab and clean up resources. | 05/03/2026 | 05/03/2026 | |\n| Monday | - Start practicing Lab 20 (Transit Gateway). Run CloudFormation to create 4 VPCs. Initialize TGW and attach the VPCs. Read TGW documentation while working. Delete the stack at the end of the day to save TGW costs. | 05/04/2026 | 05/04/2026 | |\n| Tuesday | - Recreate Lab 20 infrastructure. Start configuring Route Tables for TGW and each VPC, but the configuration is complex and testing hasn't succeeded yet. Delete resources at the end of the day. | 05/05/2026 | 05/05/2026 | |\n| Wednesday | - Recreate Lab 20 infrastructure. Review and finalize Route Table configurations, successfully test pinging across all 4 EC2 instances. Complete the lab and clean up all resources entirely. | 05/06/2026 | 05/06/2026 | |\n| Thursday | - Summarize the network configuration errors encountered. Start watching Module 03 theory lectures on YouTube to prepare for the upcoming series. | 05/07/2026 | 05/07/2026 | |\n\n