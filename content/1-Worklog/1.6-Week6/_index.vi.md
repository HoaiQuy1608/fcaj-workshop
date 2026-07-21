---
title: "Worklog Tuần 6"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6

* Học về dịch vụ RDS & Aurora của AWS, thực hành Lab 05, Lab 06 và các bài lab còn thiếu.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Đọc thêm tài liệu về RDS, Aurora và xem lại video bài giảng Module 06 để ôn lại lý thuyết trước khi thực hành. | 22/05/2026 | 22/05/2026 | [docs.aws.amazon.com (Amazon RDS)](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) - [docs.aws.amazon.com (Amazon Aurora)](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html) |
| Thứ&nbsp;Bảy | Thực hành Lab 05 về Amazon RDS: tạo RDS MySQL, cài Node.js + MySQL client trên EC2, deploy ứng dụng kết nối RDS. Gặp lỗi package mysql không tương thích MySQL 8.4, sửa bằng cách chuyển sang mysql2. | 23/05/2026 | 23/05/2026 | [awsstudygroup.com (Lab 5)](https://000005.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon RDS)](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) |
| Chủ&nbsp;Nhật | Ôn tập SQL từ cơ bản đến nâng cao: SELECT, JOIN, GROUP BY, subquery. | 24/05/2026 | 24/05/2026 | [w3schools.com (SQL)](https://www.w3schools.com/sql/) |
| Thứ&nbsp;Hai | Thực hành Lab 06 về Auto Scaling Group và Elastic Load Balancing. Fix lỗi 502 Bad Gateway bằng cách kiểm tra health check và port 5000 trong Security Group. | 25/05/2026 | 25/05/2026 | [awsstudygroup.com (Lab 6)](https://000006.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon DynamoDB)](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html) |
| Thứ&nbsp;Ba | Thực hành Lab 45 về Amazon Lightsail: deploy WordPress + Lightsail Database, cấu hình networking và firewall. Một số bước cuối bị lỗi nên chỉ đọc tài liệu. | 26/05/2026 | 26/05/2026 | [awsstudygroup.com (Lab 45)](https://000045.awsstudygroup.com/vi/) |
| Thứ&nbsp;Tư | Tìm hiểu kiến trúc tổng thể Lab 35 về Data Lake (S3, Kinesis, Glue, Athena, QuickSight). Tài khoản bị giới hạn Kinesis và Glue Crawler nên chỉ đọc tài liệu về luồng hoạt động. | 27/05/2026 | 27/05/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) |
| Thứ&nbsp;Năm | Thực hành Lab 60 về DynamoDB: tạo bảng, thao tác CRUD, Global Secondary Index bằng AWS CLI và Python SDK boto3. | 28/05/2026 | 28/05/2026 | [awsstudygroup.com (Lab 60)](https://000060.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Lightsail)](https://docs.aws.amazon.com/lightsail/) |

### Kết quả đạt được tuần 6

* Hiểu cách RDS MySQL hoạt động và cách ứng dụng Node.js kết nối đến RDS thông qua Security Group.
* Hiểu cơ chế Auto Scaling Group và Load Balancer phối hợp để cân bằng tải và tự động co giãn hệ thống.
* Nắm được cách thao tác DynamoDB bằng AWS CLI và Python SDK (boto3) và sự khác biệt giữa Query và Scan.
* Hiểu kiến trúc tổng thể của Data Lake và vai trò từng dịch vụ trong pipeline phân tích dữ liệu.
