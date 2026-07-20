---
title: "Worklog Tuần 8"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8

* Thực hành các bài lab của module 07 chưa thể thực hiện được ở tuần vừa rồi, xem và tìm hiểu các bài blog của aws, suy nghĩ ý tưởng project

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | - Tiếp tục Lab 70: Tách riêng thư mục CSV và JSON để Crawler nhận dạng đúng schema.<br>- Đọc tài liệu và xem hướng dẫn Lab 72 (Analytics on AWS). | 05/06/2026 | 05/06/2026 | |
| Thứ&nbsp;Bảy | - Bắt tay thực hành phần đầu của Lab 72.<br>- Thiết lập Glue DataBrew chuyển đổi định dạng và thử nghiệm Kinesis Data Analytics. | 06/06/2026 | 06/06/2026 | |
| Chủ&nbsp;Nhật | - Thực hành phần còn lại của Lab 72.<br>- Cấu hình Redshift Warehouse và dùng Lambda gọi dữ liệu đẩy lên. | 07/06/2026 | 07/06/2026 | |
| Thứ&nbsp;Hai | - Đọc tài liệu chuẩn bị cho Lab 73.<br>- Tìm hiểu về trực quan hóa dữ liệu (BI) sử dụng Amazon QuickSight. | 08/06/2026 | 08/06/2026 | |
| Thứ&nbsp;Ba | - Thực hành Lab 73 (Module 07).<br>- Cấu hình phân quyền truy cập S3 bucket để QuickSight có thể đọc dữ liệu an toàn. | 09/06/2026 | 10/06/2026 | |
| Thứ&nbsp;Tư | - Tiếp tục Lab 73.<br>- Giao diện QuickSight thực tế khác hoàn toàn so với tài liệu lab cũ, phải tự tìm hiểu các tính năng trên UI mới để lên được biểu đồ. | 10/06/2026 | 10/06/2026 | |
| Thứ&nbsp;Năm | - Họp nhóm suy nghĩ ý tưởng cho dự án.<br>- Nghiên cứu và tìm hiểu các chủ đề để viết bài blog chia sẻ kiến thức đăng lên group. | 11/06/2026 | 11/06/2026 | |

### Kết quả đạt được tuần 8

* Triển khai thành công pipeline phân tích dữ liệu (Analytics Pipeline) sử dụng Kinesis Data Firehose, S3, Glue Crawler, Glue Notebook (Spark), và Athena.
* Thực hiện phân tích dữ liệu cost/usage và làm sạch dữ liệu bằng Glue DataBrew và chuyển đổi định dạng CSV sang Parquet để tối ưu hiệu năng truy vấn.
* Trực quan hóa dữ liệu bằng Amazon QuickSight (thiết lập dataset, phân tích và dựng dashboard) và hiểu cách tích hợp kho dữ liệu Amazon Redshift.
* Thảo luận cùng nhóm và thống nhất các ý tưởng ban đầu cho dự án nhóm.
