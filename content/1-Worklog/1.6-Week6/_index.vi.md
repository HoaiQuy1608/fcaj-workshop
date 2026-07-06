---
title: "Worklog Tuần 6"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6:

* Học về dịch vụ RDS & Aurora của AWS, làm các bài lab liên quan và thực hành cái bài lab cũ chưa làm

### Các công việc cần triển khai trong tuần này:
| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Nghe lại Module 06 và đọc thêm tài liệu về dịch vụ RDS & Aurora | 22/05/2026 | 22/05/2026 | [youtube.com](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) - [docs.aws.amazon.com](https://docs.aws.amazon.com/rds/) |
| Thứ&nbsp;Bảy | Thực hành Lab 05 về Amazon RDS. Đã tạo RDS MySQL database, cấu hình Security Group  <br> để EC2 kết nối đến RDS, cài Node.js và MySQL client trên EC2, tạo database/table và triển  <br> khai ứng dụng Node.js kết nối đến RDS. Trong quá trình chạy app gặp lỗi do file .env rỗng  <br> và package mysql không tương thích với MySQL 8.4, đã sửa bằng cách cấu hình lại .env và  <br> chuyển sang mysql2. Cuối cùng ứng dụng chạy thành công trên port 5000 và kết nối được đến  <br> RDS. | 23/05/2026 | 23/05/2026 | [awsstudygroup.com (Lab 5)](https://000005.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=B5rOeWQWg1c&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=220) |
| Chủ&nbsp;Nhật | Ôn tập lại SQL từ các câu query cơ bản đến nâng cao | 24/05/2026 | 24/05/2026 |  |
| Thứ&nbsp;Hai | Thực hành Lab 06 về Auto Scaling Group và Elastic Load Balancing. Đã triển khai web  <br> application trên EC2, cấu hình RDS database, tạo Launch Template, Target Group, Application  <br> Load Balancer và Auto Scaling Group. Trong quá trình kiểm tra, đã xử lý lỗi 502 Bad Gateway  <br> bằng cách kiểm tra health check, port 5000 và Security Group để target chuyển sang trạng thái  <br> healthy. | 25/05/2026 | 25/05/2026 | [awsstudygroup.com (Lab 6)](https://000006.awsstudygroup.com/vi/) |
| Thứ&nbsp;Ba | Thực hành Lab 45 của Module 03 về Amazon Lightsail. Đã tạo Lightsail Database và triển khai  <br> WordPress instance, cấu hình kết nối WordPress với database thông qua DB_HOST, DB_USER,  <br> DB_PASSWORD và DB_NAME. Trong quá trình thực hiện đã xử lý lỗi kết nối database do sai  <br> endpoint/tên database. Đã tìm hiểu và cấu hình phần networking/firewall của Lightsail, kiểm tra  <br> SSH/HTTP/HTTPS rules và thực hành phần bảo mật ứng dụng. 2 instance còn lại bị lỗi ở một vài  <br> bước nên ngưng lại, chỉ đọc tài liệu các bước tạo snapshot, chuyển sang instance lớn và tạo cảnh báo. | 26/05/2026 | 26/05/2026 | [awsstudygroup.com (Lab 45)](https://000045.awsstudygroup.com/vi/) |
| Thứ&nbsp;Tư | Tìm hiểu Lab 35 của Module 07 về Data Lake on AWS. Đọc kiến trúc tổng thể của pipeline dữ liệu  <br> gồm S3, Kinesis Data Firehose, AWS Glue Data Catalog, Glue Crawler, Athena và QuickSight.  <br> Trong quá trình thực hành, tài khoản AWS bị giới hạn quyền truy cập Kinesis Data Firehose và AWS  <br> Glue Crawler nên không thể tạo Delivery Stream, chạy CloudFormation liên quan đến Kinesis hoặc  <br> tạo crawler để catalog dữ liệu. Vì vậy chuyển sang đọc hiểu luồng hoạt động của Data Lake, vai trò  <br> của từng dịch vụ. | 27/05/2026 | 27/05/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=uYCW51_pBBA&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=246) |
| Thứ&nbsp;Năm | Thực hành Lab 60 về Amazon DynamoDB. Tạo bảng DynamoDB bằng AWS CLI, ghi dữ liệu, đọc  <br> dữ liệu, cập nhật dữ liệu, truy vấn dữ liệu bằng Query/Scan, tạo và truy vấn Global Secondary Index.  <br> Sau đó sử dụng Python SDK boto3 để thực hiện các lệnh tạo, cập nhật, xóa, đọc dữ liệu, load dữ liệu  <br> mẫu, truy vấn và xóa dữ liệu. | 28/05/2026 | 28/05/2026 | [awsstudygroup.com (Lab 60)](https://000060.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=cqczgtnvHjc&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=273) |

### Kết quả đạt được tuần 6:

* Hiểu sâu hơn về cơ sở dữ liệu trên AWS bao gồm Amazon RDS, DynamoDB, Lightsail Database và các cơ chế Auto Scaling / Load Balancing.
* Triển khai thành công ứng dụng Node.js kết nối đến RDS MySQL và xử lý được các lỗi liên quan đến môi trường và phiên bản MySQL.
* Cấu hình thành công Auto Scaling Group kết hợp Application Load Balancer để tự động co giãn hệ thống và định tuyến traffic, xử lý thành công lỗi 502 Bad Gateway qua health check.
* Thực hành tạo bảng, thao tác CRUD dữ liệu và thiết lập Global Secondary Index (GSI) trên DynamoDB bằng cả AWS CLI và Python SDK (boto3).
* Triển khai được WordPress và database trên Amazon Lightsail, hiểu cách cấu hình networking và firewall cho Lightsail.
* Nắm được luồng kiến trúc Data Lake và vai trò của các dịch vụ Kinesis, S3, Glue, Athena.
