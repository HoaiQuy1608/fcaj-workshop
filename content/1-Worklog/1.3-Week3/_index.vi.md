---
title: "Worklog Tuần 3"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu tuần 3

* Hoàn thành các bài Lab 10, 19, 20 còn lại của Module 02 về Route 53, VPC Peering và Transit Gateway.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Bắt đầu Lab 10 về phân giải tên miền DNS bằng Route 53. Mẫu CloudFormation bị lỗi không dùng được nên tự mò cấu hình Inbound Endpoint và Private Hosted Zone thủ công. | 01/05/2026 | 02/05/2026 | [awsstudygroup.com (Lab 10)](https://000010.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Route 53)](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html) |
| Thứ&nbsp;Bảy | Tiếp tục fix Lab 10, nghiên cứu thêm tài liệu và nhờ AI hỗ trợ để hoàn thành phần DNS Resolution. | 02/05/2026 | 02/05/2026 | [awsstudygroup.com (Lab 10)](https://000010.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon Route 53)](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html) |
| Chủ&nbsp;Nhật | Thực hành Lab 19 về VPC Peering: cấu hình kết nối 2 VPC. Bị lỗi 2 máy EC2 không ping được nhau, dùng traceroute để dò lỗi Route Table. | 03/05/2026 | 04/05/2026 | [awsstudygroup.com (Lab 19)](https://000019.awsstudygroup.com/vi/) - [docs.aws.amazon.com (VPC Peering)](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html) |
| Thứ&nbsp;Hai | Tiếp tục fix lỗi Lab 19: sửa lại Route Table cho đúng chiều và ping thành công. | 04/05/2026 | 04/05/2026 | [awsstudygroup.com (Lab 19)](https://000019.awsstudygroup.com/vi/) - [docs.aws.amazon.com (VPC Peering)](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html) |
| Thứ&nbsp;Ba | Bắt đầu Lab 20: tạo Transit Gateway để làm trung tâm kết nối nhiều VPC thay cho VPC Peering. | 05/05/2026 | 07/05/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Transit Gateway)](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html) |
| Thứ&nbsp;Tư | Tiếp tục Lab 20: cấu hình Route Table cho Transit Gateway để mấy cái VPC thông với nhau được. | 06/05/2026 | 07/05/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon EFS)](https://docs.aws.amazon.com/efs/latest/ug/whatisefs.html) - [docs.aws.amazon.com (Amazon FSx)](https://docs.aws.amazon.com/fsx/) |
| Thứ&nbsp;Năm | Hoàn tất Lab 20: test thử và xác nhận EC2-01 ping được đến EC2-02, EC2-03, EC2-04 qua mạng nội bộ. | 07/05/2026 | 07/05/2026 | [awsstudygroup.com (Lab 20)](https://000020.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Transit Gateway)](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html) |

### Kết quả đạt được tuần 3

* Hiểu cơ chế DNS Resolution với Route 53 và cách cấu hình Inbound Endpoint, Private Hosted Zone thủ công khi CloudFormation bị lỗi.
* Hiểu cách VPC Peering hoạt động và vai trò của Route Table trong việc định tuyến traffic giữa các VPC.
* Hiểu Transit Gateway là gì và tại sao nó phù hợp hơn VPC Peering khi cần kết nối nhiều VPC cùng lúc.
