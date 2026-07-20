---
title: "Week 8 Worklog"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Week 8 Objectives

* Practice remaining Module 07 labs from last week, read AWS blogs, and brainstorm group project ideas.

### Tasks to be carried out this week

| Day | <center>Task</center> | Start Date | Completion Date | <center>Reference Material</center> |
| :---: | :--- | :---: | :---: | :--- |
| Friday | Practice Lab 35 on deploying a Data Lake consisting of Kinesis Data Firehose, S3, AWS Glue Crawler, Glue Notebook/Spark to transform data, and Athena to query processed data. Read and understood the QuickSight section only. | 06/05/2026 | 06/05/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) |
| Saturday | Practice Lab 40 on cost and usage analysis with AWS Glue and Amazon Athena. Uploaded Parquet data files to Amazon S3, created a Glue Crawler to scan the data, and created tables in the Glue Data Catalog. Used Athena to query data via SQL, and checked cost/usage information from sample data. | 06/06/2026 | 06/06/2026 | [awsstudygroup.com (Lab 40)](https://000040.awsstudygroup.com/vi/) |
| Sunday | Practice Lab 70 on building a Data Lake with custom datasets. Uploaded raw data to S3, used AWS Glue DataBrew to clean/transform the data, created a Glue Crawler to catalog the data, and ran a Glue/Spark script to convert data to Parquet format. Then used Athena to query the processed data. Because the account did not have access to Cloud9, used the laptop command prompt to do the lab, and during practice, resolved an error caused by a JSON file being mixed into the CSV dataset in the same input directory. | 06/07/2026 | 06/07/2026 | [awsstudygroup.com (Lab 70)](https://000070.awsstudygroup.com/vi/) |
| Monday | Discussed project ideas with the team, researched and explored blogs to publish on the group page. | 06/08/2026 | 06/08/2026 | [aws.amazon.com (Blog)](https://aws.amazon.com/vi/blogs/apn/unified-secrets-security-with-gitguardian-and-aws-secrets-manager/) |
| Tuesday | Practice Lab 72 on Analytics on AWS. Created S3 bucket, configured Kinesis Data Firehose to ingest sample data into S3, created Glue Crawler to catalog data, transformed data using Glue DataBrew, then queried data with Athena and practiced stream analysis using Kinesis Data Analytics. Since parts 5 and 6 were just transforming using a different method, read them only; parts 11, 12, and 13 will be completed later. | 06/09/2026 | 06/10/2026 | [awsstudygroup.com (Lab 72)](https://000072.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=7qyGJLJfhws&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=282) |
| Wednesday | Continued practicing the remaining analysis parts of Lab 72: displaying data in QuickSight, Serve with Lambda, and Data Warehouse on Redshift. | 06/10/2026 | 06/10/2026 | [awsstudygroup.com (Lab 72)](https://000072.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=7qyGJLJfhws&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=282) |
| Thursday | Practice Lab 73 on Amazon QuickSight. Created a dataset from the sales.csv file, built an analysis, and created a dashboard with basic visuals to visualize data. Due to current QuickSight UI differences compared to the lab document, self-adjusted some visual configuration steps and practiced according to the new UI. | 06/11/2026 | 06/11/2026 | [awsstudygroup.com (Lab 73)](https://000073.awsstudygroup.com/vi/) |

### Week 8 Achievements

* Successfully deployed an end-to-end big data analytics pipeline using Kinesis Data Firehose, S3, Glue Crawler, Glue Notebook (Spark), and Athena.
* Analyzed cost/usage metrics and performed custom data cleansing with Glue DataBrew, converting CSV format to Parquet to optimize query performance.
* Visualized analytics data in Amazon QuickSight (built sales datasets, analyses, and dashboards) and learned how to integrate Amazon Redshift data warehouses.
* Brainstormed and aligned with the group on initial ideas for the group project.
