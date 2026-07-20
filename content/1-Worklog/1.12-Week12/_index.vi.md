---
title: "Worklog Tuần 12"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---
### Mục tiêu tuần 12

* Lên kế hoạch, thiết lập hạ tầng mạng và chuẩn bị tài nguyên cần thiết cho dự án.
* Triển khai các dịch vụ và tiến hành chạy thử nghiệm hệ thống.
* Ghi lại toàn bộ quá trình triển khai vào báo cáo.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | - Tạo kế hoạch triển khai và cấu hình hạ tầng mạng VPC. | 03/07/2026 | 03/07/2026 |  |
| Thứ&nbsp;Bảy | - Cập nhật, hoàn thiện file kế hoạch và chuẩn bị các tài nguyên triển khai (mã nguồn, cấu hình hệ thống). | 04/07/2026 | 04/07/2026 |  |
| Chủ&nbsp;Nhật | - Triển khai giai đoạn đầu của dự án: cấu hình các tài nguyên lưu trữ và cơ sở dữ liệu gồm 2 S3 bucket, 2 bảng DynamoDB và 2 SQS queue (task queue và Dead Letter Queue). | 05/07/2026 | 05/07/2026 |  |
| Thứ&nbsp;Hai | - Tiếp tục triển khai hạ tầng: khởi tạo và cấu hình 4 Lambda function, thiết lập EventBridge Scheduler, lưu trữ API key bảo mật trong AWS Secrets Manager; sửa đổi các lỗi cấu hình và tiến hành chạy thử nghiệm hệ thống. | 06/07/2026 | 06/07/2026 |  |
| Thứ&nbsp;Ba | - Chạy thử website và phát hiện lỗi: frontend và backend không ăn khớp do Lambda thiếu logic xử lý lưu dữ liệu, thiếu bảng DynamoDB, thiếu biến môi trường. Đã khắc phục một phần bằng cách bổ sung 2 bảng DynamoDB. | 07/07/2026 | 09/07/2026 |  |
| Thứ&nbsp;Tư | - Tiếp tục khắc phục lỗi chức năng tạo test suite, sửa dropdown. Đã khắc phục lỗi API Gateway bị CORS chặn, thiếu route và authorizer. Sửa lỗi đăng nhập của Developer. | 08/07/2026 | 09/07/2026 |  |
| Thứ&nbsp;Năm | - Khắc phục nhanh lỗi dữ liệu không hiển thị trên website, giải quyết toàn bộ các vấn đề còn tồn đọng. Hệ thống đã chạy thành công. | 09/07/2026 | 09/07/2026 |  |

### Kết quả đạt được tuần 12

* Thống nhất kế hoạch triển khai chi tiết và cấu hình thành công hạ tầng mạng VPC.
* Khởi tạo và thiết lập các dịch vụ lưu trữ, cơ sở dữ liệu và hàng đợi tin nhắn: 2 S3 bucket, 2 bảng DynamoDB, 2 SQS queue (bao gồm Dead Letter Queue).
* Triển khai và cấu hình 4 Lambda function, thiết lập sự kiện kích hoạt bằng EventBridge Scheduler và lưu trữ API key an toàn bằng AWS Secrets Manager.
* Phát hiện và xử lý nhiều vấn đề nghiêm trọng khi chạy thử: mất đồng bộ giữa frontend và backend, thiếu logic Lambda, thiếu bảng DynamoDB, thiếu cấu hình API Gateway và biến môi trường.
* Khắc phục toàn bộ các vấn đề phát sinh trong quá trình debug: sửa CORS, bổ sung route, authorizer, integration cho API Gateway, sửa lỗi đăng nhập, bổ sung các bảng và biến môi trường còn thiếu.
* Chạy kiểm thử toàn bộ luồng hệ thống (thủ công và tự động) thành công, xác nhận kết quả chạy đúng và email báo cáo được gửi thành công. Hoàn thành viết báo cáo triển khai.
