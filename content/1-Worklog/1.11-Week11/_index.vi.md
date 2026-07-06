---
title: "Worklog Tuần 11"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Mục tiêu tuần 11:

* Hoàn thiện sơ đồ kiến trúc tối ưu chi phí và bảo mật cho dự án nhóm.
* Phân chia công việc thành viên và chuẩn bị môi trường triển khai.

### Các công việc cần triển khai trong tuần này:
| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Họp nhóm tối ưu sơ đồ kiến trúc: quyết định loại bỏ dịch vụ SNS do không cần thiết cho dự án nhóm, thay thế dịch vụ AWS Bedrock bằng giải pháp khác vì tài khoản Free Tier bị giới hạn, thảo luận giải pháp cấu hình luồng mạng VPC. | 26/06/2026 | 26/06/2026 |  |
| Thứ&nbsp;Bảy | Tiếp tục hoàn thiện kiến trúc cùng nhóm: điều chỉnh luồng hàng đợi SQS kích hoạt Lambda, xem xét và cấu hình giám sát hệ thống với CloudWatch. | 27/06/2026 | 27/06/2026 |  |
| Chủ&nbsp;Nhật | Cấu hình chi tiết các luồng dữ liệu trên sơ đồ kiến trúc, tập trung giải quyết phân vùng mạng cho Lambda Processing trong VPC. | 28/06/2026 | 28/06/2026 |  |
| Thứ&nbsp;Hai | Nhóm các tài nguyên liên quan trên sơ đồ kiến trúc thành các group để tăng tính trực quan. | 29/06/2026 | 29/06/2026 |  |
| Thứ&nbsp;Ba | Tiếp tục chỉnh sửa kiến trúc cùng nhóm: đặt Lambda Processing vào trong Private Subnet đi qua NAT Gateway và VPC Endpoints để giao tiếp với AI bên ngoài; hoàn thiện sơ đồ kiến trúc cuối cùng. | 30/06/2026 | 30/06/2026 |  |
| Thứ&nbsp;Tư | Phân công công việc cụ thể cho từng thành viên và thống nhất stack công nghệ Frontend (Next.js) và Backend (Python Boto3). | 01/07/2026 | 01/07/2026 |  |
| Thứ&nbsp;Năm |  | 02/07/2026 | 02/07/2026 |  |

### Kết quả đạt được tuần 11:

* Hoàn thiện sơ đồ kiến trúc chuẩn tối ưu chi phí và bảo mật: đặt ECS Fargate trong Private Subnet kết hợp với VPC Endpoints để giao tiếp nội bộ an toàn với S3, DynamoDB, ECR; đặt Lambda hậu kỳ đi qua NAT Gateway để gọi ChatGPT API.
* Phân công công việc cụ thể cho từng thành viên trong nhóm và thống nhất stack công nghệ (Next.js cho Frontend, Python Boto3 SDK cho Backend).
* Chuẩn bị sẵn sàng môi trường triển khai: Khởi tạo các IAM account, lập kế hoạch chi tiết và chuẩn bị trước các file schema dữ liệu cũng như cấu hình mạng VPC.
