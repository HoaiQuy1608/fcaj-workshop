---
title: "Worklog Tuần 5"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu tuần 5:

* Học Module 05 về bảo mật (IAM, KMS, Lambda, CloudWatch) và Module 06 về cơ sở dữ liệu.
* Thực hành các bài Lab bảo mật và giám sát hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Xem các video về dịch vụ bảo mật AWS của Module 05. Do không thể truy cập Security Hub nên chỉ đọc tài liệu Lab 18. Thực hành Lab 22 về tự động start/stop EC2 bằng Lambda: tạo EC2, gắn tag, viết code Lambda start/stop, cấu hình EventBridge Scheduler và gửi thông báo qua Slack. Đã xử lý lỗi do cấu hình sai tag EC2, sau khi chỉnh lại tag environment_auto=true và test lại code Lambda thì hệ thống hoạt động chính xác, gửi thông báo thành công lên Slack và EC2 khởi động, tắt bình thường. | 15/05/2026 | 15/05/2026 | [youtube.com](https://www.youtube.com/watch?v=tsobAlSg19g&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=150) - [youtube.com](https://www.youtube.com/watch?v=esPRIj_zZSQ&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=161) - [awsstudygroup.com (Lab 22)](https://000022.awsstudygroup.com/vi/) |
| Thứ&nbsp;Bảy | Thực hành Lab 28 về quản lý truy cập EC2 bằng Resource Tag thông qua IAM. Tạo IAM User và Role, thiết lập các IAM Policy để kiểm soát quyền xem, tạo tag, khởi tạo và quản lý EC2 dựa trên Region và Tag. Tiến hành kiểm tra quyền truy cập, thử nghiệm các case thành công và bị từ chối khi sai Region hoặc sai Tag để hiểu rõ hơn cách dùng IAM Condition kết hợp aws:RequestedRegion, aws:RequestTag và ec2:ResourceTag. | 16/05/2026 | 16/05/2026 | [awsstudygroup.com (Lab 28)](https://000028.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=vkBJ0Cxc6Nw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=177) |
| Chủ&nbsp;Nhật | Thực hành Lab 30 về IAM Permission Boundary. Tạo IAM Policy giới hạn quyền EC2 theo Region, tạo IAM User và gán quyền AmazonEC2FullAccess kết hợp với Permission Boundary. Tiến hành kiểm tra quyền truy cập của user ở các Region được phép và bị chặn ngoài boundary để hiểu cách Permission Boundary giới hạn quyền tối đa của user ngay cả khi user được gán policy có quyền rộng. | 17/05/2026 | 17/05/2026 | [youtube.com](https://www.youtube.com/watch?v=rZ2oeD0Ok5U&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=188) - [awsstudygroup.com (Lab 30)](https://000030.awsstudygroup.com/vi/) |
| Thứ&nbsp;Hai | Thực hành Lab 33 về mã hóa dữ liệu S3 bằng AWS KMS. Tạo KMS Key, cấu hình mã hóa S3 object và kiểm tra quyền truy cập. Khi user chưa có quyền phù hợp với KMS key thì không thể truy cập dữ liệu, dù object nằm trong S3. Sau khi cập nhật quyền S3/KMS phù hợp, user có thể truy cập object đã mã hóa. Hiểu rằng KMS không chỉ dùng để mã hóa dữ liệu mà còn là lớp kiểm soát quyền bổ sung khi truy cập dữ liệu đã mã hóa. <br> Thực hành Lab 44 cấu hình Trust Policy cho IAM Role giới hạn theo IP nguồn bằng aws:SourceIp và thời gian bằng aws:CurrentTime. Đã xử lý lỗi switch role do session cũ còn hiệu lực bằng cách đăng nhập lại trên trình duyệt khác. | 18/05/2026 | 18/05/2026 | [youtube.com](https://www.youtube.com/watch?v=XPUfX9proJg&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=191) - [awsstudygroup.com (Lab 33)](https://000033.awsstudygroup.com/vi/) - [youtube.com](https://www.youtube.com/watch?v=ptog1aBHeko&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=202) - [awsstudygroup.com (Lab 44)](https://000044.awsstudygroup.com/vi/) |
| Thứ&nbsp;Ba | Thực hành Lab 48 về cấu hình IAM Role cho EC2 truy cập S3 an toàn. Thử nghiệm hai cách cấp quyền: dùng Access Key/Secret Key của IAM User và dùng IAM Role gắn trực tiếp vào EC2. Hiểu rõ rủi ro bảo mật của Access Key khi upload file lên S3 và chuyển cấu hình sang dùng IAM Role cho máy chủ EC2 để ứng dụng truy cập S3 mà không cần hardcode credentials. | 19/05/2026 | 19/05/2026 | [youtube.com](https://www.youtube.com/watch?v=jk4dr_DYxWs&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=210) - [awsstudygroup.com (Lab 48)](https://000048.awsstudygroup.com/vi/) |
| Thứ&nbsp;Tư | Thực hành Lab 08 (Module 03) về Amazon CloudWatch. Triển khai lại môi trường bằng CloudFormation, thiết lập quan sát Metrics, CloudWatch Logs, Logs Insights, Metric Filter, Alarm và Dashboard. Đã xử lý lỗi do file logger.py của lab không tồn tại trên S3 bằng cách tự viết script python ghi log giả lập trên EC2 để CloudWatch Agent gửi metrics/logs lên CloudWatch theo dõi hệ thống. | 20/05/2026 | 20/05/2026 | [awsstudygroup.com (Lab 8)](https://000008.awsstudygroup.com/vi/) |
| Thứ&nbsp;Năm | Xem video bài giảng Module 06 về AWS RDS và Aurora, đồng thời đọc tài liệu nghiên cứu dịch vụ cơ sở dữ liệu. | 21/05/2026 | 22/05/2026 | [youtube.com](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) - [docs.aws.amazon.com](https://docs.aws.amazon.com/rds/) |

### Kết quả đạt được tuần 5:

* Hoàn thành nội dung thực hành liên quan đến bảo mật (IAM Policy, IAM Role, Permission Boundary, IAM Condition) để kiểm soát quyền truy cập chi tiết.
* Hiểu rõ rủi ro của Access Key và chuyển sang cấu hình IAM Role cho EC2 để đảm bảo an toàn.
* Triển khai thành công tự động hóa start/stop EC2 bằng Lambda kết hợp EventBridge Scheduler và gửi thông báo qua Slack.
* Thực hiện cấu hình mã hóa dữ liệu S3 bằng AWS KMS và phân quyền truy cập KMS Key.
* Thực hành giám sát hệ thống bằng Amazon CloudWatch (Agent, Metrics, Logs, Alarm và Dashboard).
