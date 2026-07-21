---
title: "Worklog Tuần 8"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8

* Thực hành các bài lab Module 07 còn bị hạn chế ở tuần trước và thảo luận ý tưởng dự án nhóm.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Thực hành Lab 35 về Data Lake: chạy Kinesis Data Firehose đổ dữ liệu vào S3, Glue Crawler catalog dữ liệu, xử lý bằng Glue Notebook/Spark, truy vấn bằng Athena. | 05/06/2026 | 05/06/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EFS)](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) - [docs.aws.amazon.com (Amazon FSx)](https://docs.aws.amazon.com/fsx/) |
| Thứ&nbsp;Bảy | Thực hành Lab 40: upload file Parquet lên S3, tạo Glue Crawler, truy vấn dữ liệu cost/usage bằng Athena SQL. | 06/06/2026 | 06/06/2026 | [awsstudygroup.com (Lab 40)](https://000040.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EFS)](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) - [docs.aws.amazon.com (Amazon FSx)](https://docs.aws.amazon.com/fsx/) |
| Chủ&nbsp;Nhật | Thực hành Lab 70: upload dữ liệu raw lên S3, dùng Glue DataBrew làm sạch, chuyển sang Parquet. Xử lý lỗi do file CSV lẫn JSON trong cùng thư mục input. | 07/06/2026 | 07/06/2026 | [awsstudygroup.com (Lab 70)](https://000070.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EFS)](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) - [docs.aws.amazon.com (Amazon FSx)](https://docs.aws.amazon.com/fsx/) |
| Thứ&nbsp;Hai | Họp nhóm thảo luận ý tưởng cho dự án, tìm hiểu các bài blog AWS để đăng lên group. | 08/06/2026 | 08/06/2026 | [aws.amazon.com (Secrets Security)](https://aws.amazon.com/vi/blogs/apn/unified-secrets-security-with-gitguardian-and-aws-secrets-manager/) - [aws.amazon.com (Test Automation)](https://aws.amazon.com/vi/blogs/apn/ai-powered-test-automation-with-rapise-and-amazon-bedrock/) - [aws.amazon.com (Continuous Modernization)](https://aws.amazon.com/vi/blogs/aws/proactively-reduce-tech-debt-autonomously-with-aws-transform-continuous-modernization-preview) |
| Thứ&nbsp;Ba | Bắt đầu Lab 72 về Analytics: Kinesis Firehose ingest dữ liệu, Glue Crawler catalog, DataBrew transform, Athena truy vấn, Kinesis Analytics phân tích stream. | 09/06/2026 | 10/06/2026 | [awsstudygroup.com (Lab 72)](https://000072.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Athena)](https://docs.aws.amazon.com/athena/latest/ug/what-is.html) - [docs.aws.amazon.com (AWS Glue)](https://docs.aws.amazon.com/glue/latest/dg/what-is-glue.html) |
| Thứ&nbsp;Tư | Tiếp tục Lab 72: hiển thị dữ liệu trên QuickSight, Serve with Lambda và Redshift Warehouse. | 10/06/2026 | 10/06/2026 | [awsstudygroup.com (Lab 72)](https://000072.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Athena)](https://docs.aws.amazon.com/athena/latest/ug/what-is.html) - [docs.aws.amazon.com (AWS Glue)](https://docs.aws.amazon.com/glue/latest/dg/what-is-glue.html) |
| Thứ&nbsp;Năm | Thực hành Lab 73 về QuickSight: tạo dataset từ file sales.csv, xây dựng analysis và dashboard trực quan hóa dữ liệu. | 11/06/2026 | 11/06/2026 | [awsstudygroup.com (Lab 73)](https://000073.awsstudygroup.com/vi/) |

### Kết quả đạt được tuần 8

* Hiểu cách pipeline phân tích dữ liệu vận hành từ ingestion (Kinesis) đến storage (S3), transformation (Glue/DataBrew) và querying (Athena).
* Hiểu cách QuickSight trực quan hóa dữ liệu phân tích và cách Redshift đóng vai trò data warehouse.
* Xác định được hướng ý tưởng cho dự án nhóm sau buổi thảo luận.
