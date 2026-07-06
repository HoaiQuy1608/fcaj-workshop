---
title: "Worklog Tuần 8"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8:

* Thực hành các bài lab của module 07 chưa thể thực hiện được ở tuần vừa rồi, xem và tìm hiểu các bài blog của aws, suy nghĩ ý tưởng project

### Các công việc cần triển khai trong tuần này:
| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Thực hành lab 35 về triển khai Data Lake gồm Kinesis Data Firehose, S3, AWS Glue  <br> Crawler, Glue Notebook/Spark để chuyển đổi dữ liệu và Athena để truy vấn dữ liệu  <br> đã xử lý. Phần QuickSight chỉ đọc hiểu. | 05/06/2026 | 05/06/2026 | [awsstudygroup.com (Lab 35)](https://000035.awsstudygroup.com/vi/) |
| Thứ&nbsp;Bảy | Thực hành Lab 40 về phân tích chi phí và hiệu năng sử dụng với AWS Glue và  <br> Amazon Athena. Upload các file dữ liệu Parquet lên Amazon S3, tạo Glue Crawler  <br> để scan dữ liệu và tạo table trong Glue Data Catalog. Sử dụng Athena để truy vấn  <br> dữ liệu bằng SQL, kiểm tra thông tin cost/usage từ dữ liệu mẫu. | 06/06/2026 | 06/06/2026 | [awsstudygroup.com (Lab 40)](https://000040.awsstudygroup.com/vi/) |
| Chủ&nbsp;Nhật | Thực hành Lab 70 về xây dựng Data Lake với dữ liệu tùy chỉnh. Upload dữ liệu raw  <br> lên S3, sử dụng AWS Glue DataBrew để làm sạch/chuyển đổi dữ liệu, tạo Glue Crawler  <br> để catalog dữ liệu và chạy Glue/Spark script để chuyển dữ liệu sang định dạng Parquet.  <br> Sau đó dùng Athena để truy vấn dữ liệu đã xử lý. Vì account không có quyền truy cập <br> Cloud9 nên đã sử dụng cmd của laptop để làm lab, và trong quá trình thực hành đã xử lý  <br> lỗi do dataset CSV bị lẫn file JSON trong cùng thư mục input. | 07/06/2026 | 07/06/2026 | [awsstudygroup.com (Lab 70)](https://000070.awsstudygroup.com/vi/) |
| Thứ&nbsp;Hai | Họp nhóm suy nghĩ ý tưởng cho project, nghiên cứu, tìm hiểu các bài blog để đăng lên  <br> group | 08/06/2026 | 08/06/2026 | [aws.amazon.com (Blog)](https://aws.amazon.com/vi/blogs/apn/unified-secrets-security-with-gitguardian-and-aws-secrets-manager/) |
| Thứ&nbsp;Ba | Thực hành Lab 72 về Analytics on AWS. Đã tạo S3 bucket, cấu hình Kinesis Data Firehose  <br> để ingest dữ liệu mẫu vào S3, tạo Glue Crawler để catalog dữ liệu, transform dữ liệu bằng  <br> Glue DataBrew, sau đó truy vấn dữ liệu bằng Athena và thực hành phân tích stream với  <br> Kinesis Data Analytics. Vì phần 5, 6 chỉ là transform bằng cách khác nên chỉ đọc, phần  <br> 11, 12, 13 sẽ làm sau. | 09/06/2026 | 10/06/2026 | [awsstudygroup.com (Lab 72)](https://000072.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=7qyGJLJfhws&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=282) |
| Thứ&nbsp;Tư | Tiếp tục thực hành các phần phân tích còn lại của lab 72 là hiển thị dữ liệu trong Quicksight,  <br> Serve with Lambda và Warehouse trên Redshift. | 10/06/2026 | 10/06/2026 | [awsstudygroup.com (Lab 72)](https://000072.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=7qyGJLJfhws&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=282) |
| Thứ&nbsp;Năm | Thực hành Lab 73 về Amazon QuickSight. Đã tạo dataset từ file sales.csv, xây dựng  <br> analysis và dashboard với các visual cơ bản để trực quan hóa dữ liệu. Do giao diện  <br> QuickSight hiện tại có một số điểm khác so với tài liệu lab, một số bước cấu hình visual  <br> đã tự điều chỉnh và thực hành theo UI mới. | 11/06/2026 | 11/06/2026 | [awsstudygroup.com (Lab 73)](https://000073.awsstudygroup.com/vi/) |

### Kết quả đạt được tuần 8:

* Triển khai thành công pipeline phân tích dữ liệu (Analytics Pipeline) sử dụng Kinesis Data Firehose, S3, Glue Crawler, Glue Notebook (Spark), và Athena.
* Thực hiện phân tích dữ liệu cost/usage và làm sạch dữ liệu bằng Glue DataBrew và chuyển đổi định dạng CSV sang Parquet để tối ưu hiệu năng truy vấn.
* Trực quan hóa dữ liệu bằng Amazon QuickSight (thiết lập dataset, phân tích và dựng dashboard) và hiểu cách tích hợp kho dữ liệu Amazon Redshift.
* Thảo luận cùng nhóm và thống nhất các ý tưởng ban đầu cho dự án nhóm.
