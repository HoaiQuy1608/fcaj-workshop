---
title: "Worklog Tuần 5"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu tuần 5

* Học Module 05 về bảo mật (IAM, KMS, Lambda, CloudWatch) và Module 06 về cơ sở dữ liệu.
* Thực hành các bài Lab bảo mật và giám sát hệ thống.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | - Bắt đầu Module 05 về AWS Security.<br>- Thực hành Lab 22: Tự động start/stop EC2 bằng Lambda.<br>- Xử lý lỗi do tag EC2 không khớp, cập nhật thành `environment_auto=true` và hàm Lambda chạy thành công. | 15/05/2026 | 15/05/2026 | |
| Thứ&nbsp;Bảy | - Thực hành Lab 28: Quản lý truy cập EC2 bằng Resource Tag qua IAM.<br>- Cấu hình các IAM Condition để giới hạn quyền khởi động/tắt máy chủ theo đúng tag dự án. | 16/05/2026 | 16/05/2026 | |
| Chủ&nbsp;Nhật | - Thực hành Lab 30 về IAM Permission Boundary.<br>- Áp dụng policy boundary để giới hạn quyền tối đa của user không vượt quá phạm vi Region được phép. | 17/05/2026 | 17/05/2026 | |
| Thứ&nbsp;Hai | - Thực hành Lab 33: Mã hóa dữ liệu S3 bằng AWS KMS.<br>- Thực hành Lab 44: Cấu hình Trust Policy cho IAM Role.<br>- Xử lý sự cố session cache trình duyệt khi test switch role. | 18/05/2026 | 18/05/2026 | |
| Thứ&nbsp;Ba | - Thực hành Lab 48: Cấp quyền EC2 truy cập S3.<br>- So sánh trực tiếp rủi ro bảo mật giữa việc dùng IAM Role và hardcode Access Key. | 19/05/2026 | 19/05/2026 | |
| Thứ&nbsp;Tư | - Thực hành Lab 08 (Module 03) về Amazon CloudWatch.<br>- Thiếu file `logger.py` trên S3 của bài lab, tự viết script Python giả lập đẩy log từ EC2 lên CloudWatch Log Group. | 20/05/2026 | 20/05/2026 | |
| Thứ&nbsp;Năm | - Xem các bài giảng Module 06 về Amazon RDS và Aurora.<br>- Đọc tài liệu kiến trúc Multi-AZ và Read Replica chuẩn bị cho bài lab ngày mai. | 21/05/2026 | 22/05/2026 | |

### Kết quả đạt được tuần 5

* Hoàn thành nội dung thực hành liên quan đến bảo mật (IAM Policy, IAM Role, Permission Boundary, IAM Condition) để kiểm soát quyền truy cập chi tiết.
* Hiểu rõ rủi ro của Access Key và chuyển sang cấu hình IAM Role cho EC2 để đảm bảo an toàn.
* Triển khai thành công tự động hóa start/stop EC2 bằng Lambda kết hợp EventBridge Scheduler và gửi thông báo qua Slack.
* Thực hiện cấu hình mã hóa dữ liệu S3 bằng AWS KMS và phân quyền truy cập KMS Key.
* Thực hành giám sát hệ thống bằng Amazon CloudWatch (Agent, Metrics, Logs, Alarm và Dashboard).
