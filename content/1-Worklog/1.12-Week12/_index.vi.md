---
title: "Worklog Tuần 12"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Mục tiêu tuần 12

* Triển khai toàn bộ hạ tầng và mã nguồn lên AWS.
* Kiểm thử hệ thống và hoàn thành tài liệu báo cáo.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Lên kế hoạch triển khai chi tiết và cấu hình hạ tầng mạng VPC cho dự án. | 03/07/2026 | 04/07/2026 |  |
| Thứ&nbsp;Bảy | Cập nhật và hoàn thiện file kế hoạch, chuẩn bị mã nguồn và file cấu hình cho buổi triển khai. | 04/07/2026 | 04/07/2026 |  |
| Chủ&nbsp;Nhật | Triển khai giai đoạn đầu: tạo 2 S3 Bucket, 2 bảng DynamoDB và 2 SQS Queue (Task Queue và Dead Letter Queue). | 05/07/2026 | 06/07/2026 | [console.aws.amazon.com (AWS Console)](https://console.aws.amazon.com/) |
| Thứ&nbsp;Hai | Triển khai 4 Lambda function, cấu hình EventBridge Scheduler, lưu API key vào Secrets Manager. Chạy thử và fix các lỗi cấu hình phát sinh. | 06/07/2026 | 06/07/2026 | [console.aws.amazon.com (AWS Console)](https://console.aws.amazon.com/) |
| Thứ&nbsp;Ba | Phát hiện nhiều vấn đề nghiêm trọng: Lambda thiếu logic xử lý, thiếu bảng DynamoDB, thiếu biến môi trường. Bổ sung 2 bảng DynamoDB mới và fix một phần lỗi. | 07/07/2026 | 09/07/2026 | [docs.aws.amazon.com (API Gateway CORS)](https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-cors.html) |
| Thứ&nbsp;Tư | Fix tiếp: sửa API Gateway (CORS, thiếu route, authorizer, integration), sửa lỗi đăng nhập Developer, hiển thị được dữ liệu lên website. | 08/07/2026 | 09/07/2026 | [docs.aws.amazon.com (API Gateway CORS)](https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-cors.html) |
| Thứ&nbsp;Năm | Sửa dứt điểm luồng kiểm thử thủ công và tự động. Chạy thử toàn hệ thống thấy kết quả đúng và email báo cáo gửi thành công. Hoàn thành viết tài liệu báo cáo triển khai. | 09/07/2026 | 09/07/2026 | [docs.aws.amazon.com (API Gateway CORS)](https://docs.aws.amazon.com/apigateway/latest/developerguide/how-to-cors.html) |

### Kết quả đạt được tuần 12

* Hiểu quy trình triển khai hệ thống Serverless end-to-end trên AWS từ mạng, lưu trữ, xử lý đến API.
* Hiểu nguyên nhân và cách xử lý các lỗi CORS, authorizer, integration trong API Gateway.
* Nắm được cách debug lỗi đồng bộ giữa Frontend và Backend trong hệ thống phân tán.
* Hiểu cách EventBridge, SQS và Lambda phối hợp để tự động kích hoạt luồng kiểm thử.
