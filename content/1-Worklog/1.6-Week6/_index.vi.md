---
title: "Worklog Tuần 6"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6

* Học về dịch vụ RDS & Aurora của AWS, làm các bài lab liên quan và thực hành cái bài lab cũ chưa làm

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | - Xem lại video bài giảng Module 06.<br>- Đọc thêm tài liệu kỹ thuật về kiến trúc, tính năng của dịch vụ Amazon RDS & Aurora. | 22/05/2026 | 22/05/2026 | |
| Thứ&nbsp;Bảy | - Thực hành Lab 05 về Amazon RDS.<br>- Gặp lỗi file `.env` rỗng và package mysql không tương thích chuẩn xác thực mới của MySQL 8.4.<br>- Cấu hình lại và đổi sang thư viện `mysql2` để kết nối thành công. | 23/05/2026 | 23/05/2026 | |
| Chủ&nbsp;Nhật | - Dành thời gian ôn tập lại cú pháp SQL.<br>- Thử nghiệm các câu query truy xuất và join bảng cơ bản trên RDS instance vừa tạo. | 24/05/2026 | 24/05/2026 | |
| Thứ&nbsp;Hai | - Thực hành Lab 06 (Module 03) về Auto Scaling Group (ASG) và Elastic Load Balancing (ELB).<br>- Gặp lỗi 502 Bad Gateway do Health Check thất bại.<br>- Kiểm tra lại port 5000 và Security Group, chỉnh sửa để Target Group xanh. | 25/05/2026 | 25/05/2026 | |
| Thứ&nbsp;Ba | - Thực hành Lab 45 (Module 03) về Amazon Lightsail.<br>- Xử lý lỗi ứng dụng không nhận database do sai endpoint và DB name. | 26/05/2026 | 26/05/2026 | |
| Thứ&nbsp;Tư | - Thực hành Lab 60 về Amazon DynamoDB.<br>- Dùng AWS CLI và Python SDK (boto3) thực thi các lệnh CRUD và tạo Global Secondary Index (GSI). | 27/05/2026 | 27/05/2026 | |
| Thứ&nbsp;Năm | - Bắt đầu đọc tài liệu Lab 35 (Module 07) về Data Lake.<br>- Do tài khoản lab bị chặn quyền tạo Kinesis Data Firehose nên chỉ đọc tài liệu để hiểu luồng dữ liệu. | 28/05/2026 | 28/05/2026 | |

### Kết quả đạt được tuần 6

* Hiểu sâu hơn về cơ sở dữ liệu trên AWS bao gồm Amazon RDS, DynamoDB, Lightsail Database và các cơ chế Auto Scaling / Load Balancing.
* Triển khai thành công ứng dụng Node.js kết nối đến RDS MySQL và xử lý được các lỗi liên quan đến môi trường và phiên bản MySQL.
* Cấu hình thành công Auto Scaling Group kết hợp Application Load Balancer để tự động co giãn hệ thống và định tuyến traffic, xử lý thành công lỗi 502 Bad Gateway qua health check.
* Thực hành tạo bảng, thao tác CRUD dữ liệu và thiết lập Global Secondary Index (GSI) trên DynamoDB bằng cả AWS CLI và Python SDK (boto3).
* Triển khai được WordPress và database trên Amazon Lightsail, hiểu cách cấu hình networking và firewall cho Lightsail.
* Nắm được luồng kiến trúc Data Lake và vai trò của các dịch vụ Kinesis, S3, Glue, Athena.
