---
title: "Worklog Tuần 10"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu tuần 10

* Hoàn thiện bản mô tả dự án và vẽ sơ đồ kiến trúc chi tiết.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Tiếp tục và hoàn thiện bản mô tả chi tiết đề tài dự án: luồng hoạt động tổng thể, phân tích từng dịch vụ AWS sẽ dùng. | 19/06/2026 | 19/06/2026 | |
| Thứ&nbsp;Bảy | Bắt đầu vẽ sơ đồ kiến trúc: xác định các dịch vụ AWS và vị trí trong từng lớp (Frontend, Backend, Database, Networking). | 20/06/2026 | 25/06/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Chủ&nbsp;Nhật | Kết nối các luồng dữ liệu giữa CloudFront, API Gateway, Lambda, SQS, ECS, DynamoDB trên sơ đồ. | 21/06/2026 | 25/06/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Thứ&nbsp;Hai | Bổ sung lớp bảo mật vào sơ đồ (Cognito, IAM Role, Security Group, VPC) và rà soát lại toàn bộ các luồng. | 22/06/2026 | 25/06/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Thứ&nbsp;Ba | Hoàn thiện sơ đồ và đưa lên group cho anh/chị admin xem. Nhận feedback còn sai khá nhiều lỗi cấu hình, họp nhóm bàn cách sửa. | 23/06/2026 | 25/06/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Thứ&nbsp;Tư | Họp nhóm tiếp thu feedback và điều chỉnh lại các luồng kết nối bị sai trong sơ đồ. | 24/06/2026 | 25/06/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |
| Thứ&nbsp;Năm | Sửa lỗi dựa trên feedback: fix thành công luồng kết nối từ User đến CloudFront, S3 và Internet Gateway. | 25/06/2026 | 25/06/2026 | [aws.amazon.com (AWS Architecture Icons)](https://aws.amazon.com/architecture/icons/) - [draw.io (Diagrams.net)](https://app.diagrams.net/) |

### Kết quả đạt được tuần 10

* Hoàn thành bản mô tả dự án chi tiết với đầy đủ luồng hoạt động và phân tích dịch vụ AWS.
* Hiểu rõ hơn về các lỗi thiết kế kiến trúc phổ biến sau khi nhận feedback từ anh/chị admin.
* Nắm được cách luồng dữ liệu từ phía người dùng đi qua CloudFront, S3 đến các dịch vụ backend.
