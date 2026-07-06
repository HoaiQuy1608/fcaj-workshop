---
title: "Worklog Tuần 4"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4:

* Học nội dung Module 03 và Module 04 về máy chủ EC2 và các dịch vụ lưu trữ.
* Thực hành các bài Lab liên quan đến AWS Backup và Systems Manager.

### Các công việc cần triển khai trong tuần này:
| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Xem các bài giảng lý thuyết Module 03 trên YouTube. | 08/05/2026 | 08/05/2026 | [youtube.com](https://www.youtube.com/watch?v=-t5h4N6vfBs&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=72) - [youtube.com](https://www.youtube.com/watch?v=e7XeKdOVq40&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=73) |
| Thứ&nbsp;Bảy | Xem video hướng dẫn và thực hành Lab 13 thuộc Module 04 về triển khai tự động hóa AWS Backup cho hệ thống bằng CloudFormation kết hợp với SNS và Lambda. | 09/05/2026 | 09/05/2026 | [youtube.com](https://www.youtube.com/watch?v=IHxgFMlL3y8&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=107) |
| Chủ&nbsp;Nhật | Xem video thực hành Lab 24 và Lab 57 của Module 04. Do tài khoản chưa xác minh hoàn toàn nên không truy cập được dịch vụ Storage Gateway và chỉ đọc tài liệu lý thuyết. Với Lab 57, chỉ tạo được S3 Bucket để mở trang web tĩnh, còn phần CloudFront chỉ đọc tài liệu do giới hạn tài khoản. | 10/05/2026 | 10/05/2026 | [youtube.com](https://www.youtube.com/watch?v=B3R87qxarWk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=121) -[youtube.com](https://www.youtube.com/watch?v=YPqB11Jhu8g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=137) |
| Thứ&nbsp;Hai | Xem các video bài giảng của Module 04 trên YouTube về các giải pháp lưu trữ của AWS. | 11/05/2026 | 11/05/2026 | [youtube.com](https://www.youtube.com/watch?v=hsCfP0IxoaM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=103) - |
| Thứ&nbsp;Ba | Ôn tập lại Module 04, đọc tài liệu chuẩn bị làm các bài lab và xem lại các bài lab còn thiếu của các module trước như Lab 58 của Module 02 và các bài lab Module 03 để thực hành sau. | 12/05/2026 | 12/05/2026 | [youtube.com](https://www.youtube.com/watch?v=hsCfP0IxoaM&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=103) |
| Thứ&nbsp;Tư | Thực hành Lab 58 (Module 02) về Amazon Systems Manager Session Manager. Đã tạo Public Linux EC2 và Private Windows EC2, gán IAM Role, tạo các VPC Endpoints để kết nối EC2 private bằng Session Manager. Gặp lỗi Private Windows EC2 không hiện trong Managed Nodes do security group của endpoint thiếu rule inbound HTTPS 443; sau khi bổ sung rule thì kết nối thành công và kiểm tra bằng lệnh ipconfig. Thực hành Lab 27 về quản lý tài nguyên bằng Tag và Resource Group để phân loại tài nguyên theo dự án nhóm và cleanup hiệu quả. | 13/05/2026 | 13/05/2026 | [awsstudygroup.com (Lab 58)](https://000058.awsstudygroup.com/vi/) - <br> [awsstudygroup.com (Lab 27)](https://000027.awsstudygroup.com/vi/) |
| Thứ&nbsp;Năm | Thực hành Lab 04 về Amazon EC2. Triển khai tạo Windows EC2 và Linux EC2, cấu hình Security Group để kết nối RDP/SSH, tải file Remote Desktop và kết nối thành công vào Windows EC2. Thực hành các thao tác quản lý EC2 như thay đổi cấu hình instance, tạo Snapshot, tạo Custom AMI và khởi chạy instance mới từ AMI. | 14/05/2026 | 14/05/2026 | [awsstudygroup.com (Lab 4)](https://000004.awsstudygroup.com/vi/) |

### Kết quả đạt được tuần 4:

* Hoàn thành nội dung Module 03, Module 04 về Amazon EC2 và các dịch vụ lưu trữ (S3, EBS, EFS).
* Thực hành thành công Lab 13 thiết lập AWS Backup để tự động sao lưu dữ liệu.
* Thực hành Lab 58 về AWS Systems Manager Session Manager để kết nối an toàn vào EC2 private.
* Thực hành Lab 27 về quản lý tài nguyên bằng Tag và Resource Group.
* Thực hành Lab 04 về Amazon EC2 (tạo Windows/Linux EC2, cấu hình Security Group, tạo Snapshot và Custom AMI).
