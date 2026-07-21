---
title: "Worklog Tuần 11"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Mục tiêu tuần 11

* Tối ưu kiến trúc về mặt bảo mật và chi phí.
* Thống nhất stack công nghệ và bắt đầu chuẩn bị triển khai.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Họp nhóm tối ưu sơ đồ: bỏ SNS vì không cần thiết, thay Bedrock bằng giải pháp khác do Free Tier không cho phép. | 26/06/2026 | 30/06/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Thứ&nbsp;Bảy | Tiếp tục chỉnh kiến trúc: điều chỉnh luồng SQS kích hoạt Lambda và cấu hình giám sát CloudWatch. | 27/06/2026 | 30/06/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Chủ&nbsp;Nhật | Cấu hình phân vùng mạng: đặt Lambda Processing vào Private Subnet, dùng NAT Gateway để gọi API bên ngoài và VPC Endpoints để giao tiếp nội bộ với S3, DynamoDB, ECR. | 28/06/2026 | 30/06/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Thứ&nbsp;Hai | Thêm Cognito vào kiến trúc để phân quyền người dùng, nhóm lại các tài nguyên liên quan trên sơ đồ cho rõ ràng. | 29/06/2026 | 30/06/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Thứ&nbsp;Ba | Hoàn thiện sơ đồ kiến trúc cuối cùng, phân công công việc cụ thể từng thành viên và thống nhất stack: Frontend Next.js, Backend Python Boto3. | 30/06/2026 | 30/06/2026 | [docs.aws.amazon.com (Amazon Cognito)](https://docs.aws.amazon.com/cognito/latest/developerguide/what-is-amazon-cognito.html) - [aws.amazon.com (Well-Architected)](https://aws.amazon.com/architecture/well-architected/) |
| Thứ&nbsp;Tư | Bắt đầu viết mã nguồn Backend: setup project Python, viết các hàm API và cấu hình kết nối đến các dịch vụ AWS. | 01/07/2026 | 02/07/2026 | [boto3.amazonaws.com (Boto3 Docs)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) |
| Thứ&nbsp;Năm | Khởi tạo IAM account cho từng thành viên, lập kế hoạch triển khai chi tiết và chuẩn bị file schema DynamoDB cùng cấu hình VPC cho tuần triển khai. | 02/07/2026 | 02/07/2026 | [boto3.amazonaws.com (Boto3 Docs)](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) |

### Kết quả đạt được tuần 11

* Hiểu tại sao cần đặt Lambda vào Private Subnet và dùng NAT Gateway thay vì để Lambda ra ngoài Internet trực tiếp.
* Hiểu vai trò của VPC Endpoints trong việc giúp tài nguyên trong Private Subnet giao tiếp với S3, DynamoDB mà không cần đi qua Internet.
* Nắm được lý do chọn Next.js cho Frontend và Python Boto3 cho Backend trong bối cảnh dự án.
