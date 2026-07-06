---
title: "Worklog Tuần 12"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Mục tiêu tuần 12:

* Lên kế hoạch, thiết lập hạ tầng mạng và chuẩn bị tài nguyên cần thiết cho dự án.
* Triển khai các dịch vụ và tiến hành chạy thử nghiệm hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Tạo kế hoạch triển khai và cấu hình hạ tầng mạng VPC. | 03/07/2026 | 03/07/2026 |  |
| Thứ&nbsp;Bảy | Cập nhật, hoàn thiện file kế hoạch và chuẩn bị các tài nguyên triển khai (mã nguồn, cấu hình hệ thống). | 04/07/2026 | 04/07/2026 |  |
| Chủ&nbsp;Nhật | Triển khai giai đoạn đầu của dự án: cấu hình các tài nguyên lưu trữ và cơ sở dữ liệu gồm 2 S3 bucket, 2 bảng DynamoDB và 2 SQS queue (task queue và Dead Letter Queue). | 05/07/2026 | 05/07/2026 |  |
| Thứ&nbsp;Hai | Tiếp tục triển khai hạ tầng: khởi tạo và cấu hình 4 Lambda function, thiết lập EventBridge Scheduler, lưu trữ API key bảo mật trong AWS Secrets Manager; sửa đổi các lỗi cấu hình và tiến hành chạy thử nghiệm hệ thống. | 06/07/2026 | 06/07/2026 |  |
| Thứ&nbsp;Ba |  | 07/07/2026 | 07/07/2026 |  |
| Thứ&nbsp;Tư |  | 08/07/2026 | 08/07/2026 |  |
| Thứ&nbsp;Năm |  | 09/07/2026 | 09/07/2026 |  |

### Kết quả đạt được tuần 12:

* Thống nhất kế hoạch triển khai chi tiết và cấu hình thành công hạ tầng mạng VPC.
* Khởi tạo và thiết lập các dịch vụ lưu trữ, cơ sở dữ liệu và hàng đợi tin nhắn: 2 S3 bucket, 2 bảng DynamoDB, 2 SQS queue (bao gồm Dead Letter Queue).
* Triển khai và cấu hình 4 Lambda function, thiết lập sự kiện kích hoạt bằng EventBridge Scheduler và lưu trữ API key an toàn bằng AWS Secrets Manager.
* sửa các lỗi cấu hình phát sinh khi triển khai và thử nghiệm hệ thống thành công.
