---
title: "Worklog Tuần 5"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu tuần 5

* Học Module 05 về bảo mật AWS (IAM, KMS, Lambda, CloudWatch).
* Thực hành nhiều bài lab bảo mật và giám sát hệ thống.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Xem video Module 05 về bảo mật AWS. Thực hành Lab 22: viết Lambda tự động start/stop EC2 theo tag, cấu hình EventBridge Scheduler, gửi thông báo Slack. | 15/05/2026 | 15/05/2026 | [awsstudygroup.com (Lab 22)](https://000022.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Auto Scaling)](https://docs.aws.amazon.com/autoscaling/ec2/userguide/what-is-amazon-ec2-auto-scaling.html) - [docs.aws.amazon.com (ELB)](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html) |
| Thứ&nbsp;Bảy | Thực hành Lab 28: tạo IAM User/Role với IAM Policy kiểm soát quyền EC2 theo Region và Tag, thử nghiệm các case được và bị từ chối để hiểu rõ IAM Condition. | 16/05/2026 | 16/05/2026 | [awsstudygroup.com (Lab 28)](https://000028.awsstudygroup.com/vi/) - [docs.aws.amazon.com (IAM Policies)](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html) |
| Chủ&nbsp;Nhật | Thực hành Lab 30: cấu hình Permission Boundary giới hạn quyền tối đa của IAM User dù được gán policy rộng. | 17/05/2026 | 17/05/2026 | [awsstudygroup.com (Lab 30)](https://000030.awsstudygroup.com/vi/) - [docs.aws.amazon.com (IAM Policies)](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html) |
| Thứ&nbsp;Hai | Thực hành Lab 33: mã hóa S3 object bằng AWS KMS, phân quyền truy cập KMS Key. Thực hành Lab 44: tạo Trust Policy giới hạn truy cập theo IP nguồn và thời gian. | 18/05/2026 | 18/05/2026 | [awsstudygroup.com (Lab 33)](https://000033.awsstudygroup.com/vi/) - [awsstudygroup.com (Lab 44)](https://000044.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS KMS)](https://docs.aws.amazon.com/kms/latest/developerguide/overview.html) |
| Thứ&nbsp;Ba | Thực hành Lab 48: so sánh 2 cách cấp quyền EC2 truy cập S3 (Access Key vs. IAM Role), hiểu rủi ro bảo mật khi hardcode credentials. | 19/05/2026 | 19/05/2026 | [awsstudygroup.com (Lab 48)](https://000048.awsstudygroup.com/vi/) |
| Thứ&nbsp;Tư | Thực hành Lab 08 về CloudWatch: deploy môi trường bằng CloudFormation, tự viết script Python giả lập log trên EC2 (file logger.py gốc không có trên S3), thiết lập Metric, Alarm, Dashboard. | 20/05/2026 | 20/05/2026 | [awsstudygroup.com (Lab 8)](https://000008.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon CloudWatch)](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html) |
| Thứ&nbsp;Năm | Xem video Module 06 về AWS RDS và Aurora, đọc tài liệu chuẩn bị cho tuần sau. | 21/05/2026 | 21/05/2026 | [docs.aws.amazon.com (Amazon RDS)](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) - [docs.aws.amazon.com (Amazon Aurora)](https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/CHAP_AuroraOverview.html) |

### Kết quả đạt được tuần 5

* Hiểu cách IAM Policy, IAM Condition, Permission Boundary hoạt động để kiểm soát quyền truy cập chi tiết.
* Hiểu rủi ro bảo mật khi dùng Access Key và tại sao IAM Role gắn vào EC2 là cách làm đúng đắn hơn.
* Hiểu cách KMS mã hóa dữ liệu S3 và đóng vai trò là lớp kiểm soát quyền bổ sung.
* Nắm được cách CloudWatch thu thập metrics/logs từ EC2 và cách cấu hình Alarm, Dashboard giám sát hệ thống.
