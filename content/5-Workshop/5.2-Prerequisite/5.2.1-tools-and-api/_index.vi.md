---
title : "Công cụ & API Key"
date : 2026-07-10
weight : 1
chapter : false
pre : " <b> 5.2.1. </b> "
---

#### Các công cụ và tài nguyên cần thiết

Trước khi bắt đầu tiến hành xây dựng hệ thống Playwright Serverless, bạn cần chuẩn bị các tài nguyên sau:

**1. Tài khoản AWS (AWS Account)**

- Bạn cần có quyền truy cập vào AWS Management Console.
- Khuyến nghị sử dụng tài khoản có quyền Quản trị viên (Administrator Access) để thực hiện bài Lab này một cách trơn tru nhất.

**2. Mã nguồn (Source Code)**

- Bạn cần tải các mã nguồn đã được đóng gói sẵn để sử dụng cho Giao diện (Frontend) và phần xử lý (Backend).
- Tải các file mã nguồn tại đây:

| File | Mô tả |
| ------ | ------- |
| [lambda-backend.zip](/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/lambda-backend.zip) | Lambda function xử lý backend chính |
| [lambda-coordinator.zip](/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/lambda-coordinator.zip) | Lambda function điều phối (Coordinator) |
| [lambda-error-handler.zip](/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/lambda-error-handler.zip) | Lambda function xử lý lỗi (Error Handler) |
| [lambda-postprocessing.zip](/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/lambda-postprocessing.zip) | Lambda function hậu xử lý (Post-processing) |
| [Mã nguồn Frontend](https://github.com/Trannhi810/cloud-native-playwright-testing.git) | Source code Giao diện Frontend (React) để build |

> [!NOTE]
> **Đối với Mã nguồn Frontend:** Bạn hãy sử dụng lệnh `git clone https://github.com/Trannhi810/cloud-native-playwright-testing.git` để tải source code về máy, sau đó tiến hành chỉnh sửa file cấu hình và build mã nguồn theo hướng dẫn ở **[5.10. Giao diện Frontend](../../5.10-frontend/)**.
>
> **Đối với các file `.zip` Lambda:** Upload trực tiếp (không cần giải nén) khi triển khai từng Lambda function ở các phần tương ứng.

**3. Khóa API Google Gemini (Gemini API Key)**

Để hệ thống có thể tự động phân tích log lỗi thông qua AI, bạn cần cung cấp một API Key từ Google. Hãy làm theo các bước sau để khởi tạo:

**Bước 1:** Truy cập vào trang [Google AI Studio](https://aistudio.google.com/app/apikey) và đăng nhập bằng tài khoản Google của bạn.

![Truy cập Google AI Studio](/images/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/1-access-google-ai-studio.png?featherlight=false&width=90pc)

**Bước 2:** Tại giao diện chính, bấm chọn nút **Create API key** (Tạo khóa API).

![Tạo API Key](/images/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/2-create-api-key.png?featherlight=false&width=90pc)

**Bước 3:** Sao chép (Copy) chuỗi mã khóa vừa được tạo. Hãy lưu khóa này lại một nơi an toàn (như Notepad) để điền vào cấu hình biến môi trường của AWS Lambda ở các phần thực hành tiếp theo.

![Sao chép API Key](/images/5-Workshop/5.2-Prerequisite/5.2.1-tools-and-api/3-copy-api-key.png?featherlight=false&width=90pc)

---

Bước chuẩn bị công cụ và API Key đã hoàn tất. Tiếp theo, chúng ta sẽ chuyển sang **[5.2.2. Khởi tạo VPC](../5.2.2-create-vpc/)** để xây dựng hạ tầng mạng riêng cho hệ thống.
