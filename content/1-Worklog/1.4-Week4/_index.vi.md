---
title: "Worklog Tuần 4"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4

* Học lý thuyết Module 03, Module 04 về EC2 và lưu trữ.
* Thực hành Lab 13, Lab 57, Lab 58, Lab 04 và Lab 27.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Xem video bài giảng Module 03 và Module 04 về máy chủ EC2, S3, EBS, EFS. | 08/05/2026 | 08/05/2026 | [docs.aws.amazon.com (Amazon EC2)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) - [docs.aws.amazon.com (Amazon S3)](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html) |
| Thứ&nbsp;Bảy | Bắt đầu Lab 13 về tự động hóa AWS Backup: chạy CloudFormation tạo môi trường, setup Backup Vault và Backup Plan cơ bản. | 09/05/2026 | 10/05/2026 | [awsstudygroup.com (Lab 13)](https://000013.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS Backup)](https://docs.aws.amazon.com/aws-backup/latest/devguide/whatisbackup.html) |
| Chủ&nbsp;Nhật | Hoàn tất Lab 13: cấu hình SNS gửi thông báo và viết Lambda xử lý event sao lưu tự động. Thực hành Lab 57: tạo S3 Bucket host web tĩnh, phần CloudFront chỉ đọc tài liệu do tài khoản bị giới hạn. | 10/05/2026 | 10/05/2026 | [awsstudygroup.com (Lab 57)](https://000057.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon CloudFront)](https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html) |
| Thứ&nbsp;Hai | Đọc tài liệu ôn tập về IAM Role, VPC Endpoints và Session Manager để chuẩn bị cho Lab 58. | 11/05/2026 | 13/05/2026 | [docs.aws.amazon.com](https://docs.aws.amazon.com) |
| Thứ&nbsp;Ba | Bắt đầu Lab 58 (Session Manager): tạo IAM Role, khởi tạo Public Linux EC2 và Private Windows EC2. | 12/05/2026 | 13/05/2026 | [awsstudygroup.com (Lab 58)](https://000058.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS Systems Manager)](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html) |
| Thứ&nbsp;Tư | Tiếp tục Lab 58: cấu hình VPC Endpoints. Con Windows EC2 không hiện trong Managed Nodes, mò ra do thiếu rule HTTPS 443 trong Security Group, thêm vô là kết nối được ngay. | 13/05/2026 | 13/05/2026 | [awsstudygroup.com (Lab 58)](https://000058.awsstudygroup.com/vi/) - [docs.aws.amazon.com (AWS Systems Manager)](https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html) |
| Thứ&nbsp;Năm | Thực hành Lab 27 (gắn Tag quản lý tài nguyên) và Lab 04 (tạo Windows/Linux EC2, Snapshot, Custom AMI). | 14/05/2026 | 14/05/2026 | [awsstudygroup.com (Lab 27)](https://000027.awsstudygroup.com/vi/) - [awsstudygroup.com (Lab 4)](https://000004.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EC2)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html) |

### Kết quả đạt được tuần 4

* Hiểu quy trình tự động hóa sao lưu AWS Backup kết hợp CloudFormation, SNS và Lambda.
* Hiểu cách Session Manager hoạt động và tại sao VPC Endpoints cần thiết để kết nối EC2 private mà không cần public IP.
* Nắm được cách S3 dùng để host web tĩnh và vai trò của CloudFront trong việc phân phối nội dung.
* Hiểu cách Tag và Resource Group giúp phân loại và quản lý tài nguyên AWS hiệu quả.
