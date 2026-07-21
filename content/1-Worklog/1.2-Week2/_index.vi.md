---
title: "Worklog Tuần 2"
date: 2026-04-24
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---
### Mục tiêu tuần 2

* Nắm vững kiến trúc VPC: Subnet, Route Table, Internet Gateway, Security Group.
* Triển khai Lab 03 và kết nối EC2 trong VPC.

### Các công việc cần triển khai trong tuần này

| Thứ | <center>Công việc</center> | Ngày bắt đầu | Ngày hoàn thành | <center>Nguồn tài liệu</center> |
| :---: | :--- | :---: | :---: | :--- |
| Thứ&nbsp;Sáu | Xem video Module 02 về VPC và bắt đầu Lab 03: tạo VPC, chia Subnet public và private. | 24/04/2026 | 27/04/2026 | [awsstudygroup.com (Lab 3)](https://000003.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon VPC)](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| Thứ&nbsp;Bảy | Tiếp tục Lab 03: tạo Internet Gateway, Route Table và cấu hình để Subnet public ra được Internet. | 25/04/2026 | 27/04/2026 | [awsstudygroup.com (Lab 3)](https://000003.awsstudygroup.com/vi/) - [docs.aws.amazon.com (Amazon VPC)](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) |
| Chủ&nbsp;Nhật | Xem video về VPC Security (Security Group, NACL), cấu hình Security Group cho Lab 03. | 26/04/2026 | 27/04/2026 | [docs.aws.amazon.com (VPC Security)](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Security.html) |
| Thứ&nbsp;Hai | Tự triển khai lại toàn bộ flow của Lab 03: VPC → Subnet → IGW → Route Table → Security Group. | 27/04/2026 | 27/04/2026 | [awsstudygroup.com (Lab 3)](https://000003.awsstudygroup.com/vi/) |
| Thứ&nbsp;Ba | Triển khai máy chủ EC2 trong VPC vừa tạo và kết nối bằng EC2 Instance Connect Endpoint. | 28/04/2026 | 28/04/2026 | [awsstudygroup.com (Lab 3)](https://000003.awsstudygroup.com/vi/) - [docs.aws.amazon.com (EC2 Instance Connect)](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Connect-using-EC2-Instance-Connect.html) |
| Thứ&nbsp;Tư | Xem video hướng dẫn Lab 10 (Route 53 DNS Resolution) và đọc tài liệu chuẩn bị thực hành. | 29/04/2026 | 29/04/2026 | [docs.aws.amazon.com (Amazon Route 53)](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html) |
| Thứ&nbsp;Năm | Xem video hướng dẫn Lab 19 (VPC Peering) và Lab 20 (Transit Gateway), đọc tài liệu để chuẩn bị cho tuần tới. | 30/04/2026 | 30/04/2026 | [docs.aws.amazon.com (VPC Peering)](https://docs.aws.amazon.com/vpc/latest/peering/what-is-vpc-peering.html) - [docs.aws.amazon.com (Transit Gateway)](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html) |

### Kết quả đạt được tuần 2

* Hiểu rõ khái niệm VPC, Subnet, Internet Gateway, Route Table và cách các thành phần này liên kết với nhau.
* Hiểu cách EC2 Instance Connect Endpoint cho phép kết nối an toàn vào EC2 private mà không cần public IP.
* Nắm được tổng quan kiến trúc của các bài Lab 10, 19, 20 để chuẩn bị thực hành.
