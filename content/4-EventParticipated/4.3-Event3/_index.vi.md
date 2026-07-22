---
title: "FCAJ Community Day (Data Driven, AI Risen)"
date: 2026-06-27
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---



### Mục Đích Của Sự Kiện

- Khám phá các hệ thống quản lý hoạt động đám mây tự động và kiến trúc của Deep Response Engine.
- Tìm hiểu về Voice Agents và cách xây dựng các hệ thống giao tiếp bằng giọng nói sử dụng AI ở quy mô doanh nghiệp.
- Giới thiệu AWS DevOps Agent và phương pháp tối ưu hóa vận hành thông qua Multi-Agent.
- Phân tích hiệu quả của việc ứng dụng AI vào quy hoạch nhân sự (Workforce Planning) tại doanh nghiệp với Amazon Quick.
- Hướng dẫn thiết lập kết nối an toàn bảo mật thông qua giao thức MCP (Model Context Protocol) với Amazon Quick.

### Danh Sách Diễn Giả

- **Truong Tran** - AI Solution Sales, Noventiq
- **Steve Tran** - CTO/Founder, CloudThinker
- **Trung Vu** - CEO, Revve AI
- **Anh Dang** - Solution Sales, Noventiq
- **Nghi Danh** - AI Engineer, Renova Cloud
- **Kiet Tran** - AI Engineer, AWS Student Builder Group
- **Bao Phan** - Cloud Engineer, Cloud Kinetics
- **Nguyen Nguyen** - Cloud Engineer, Cloud Kinetics
- **Toan Nguyen** - AWS Security Builder

### Nội Dung Nổi Bật

#### 1. AgenticOps for your Cloud (AgenticOps cho Đám mây của bạn)
- **Diễn giả:** Steve Tran
- **Nghịch lý vận hành Đám mây:** Sự tiến hóa công nghệ làm tăng 4x công cụ và 3x nhân sự, nhưng thời gian xử lý sự cố (MTTR) không đổi. Kỹ sư liên tục bị quá tải trước "Bức tường phức tạp" (Complexity Wall).
- **Giải pháp Enterprise AgenticOps:** Xây dựng hệ sinh thái AI gồm nhiều Agent chuyên biệt (Cloud, Kubernetes, Security, Database...) được điều phối bởi Super Agent để tự động hóa các tác vụ phức tạp thay con người.
- **Quan điểm cốt lõi:** Chuyển từ hệ thống chỉ biết cảnh báo (Observability) sang hệ thống tự động hành động và học hỏi ("CloudThinker acts on it. learn it.").
- **Giá trị thực tế (ROI):** 
  - Giảm 87% MTTR, tự động giải quyết 70% sự cố (scale team SRE không cần thêm người).
  - Thu hồi 10-25% tài nguyên đám mây lãng phí, giảm OPEX.
  - Giảm thiểu 40% thời gian làm các tác vụ nhàm chán (Toil).

#### 2. Building Voice Agent at Scale (Xây dựng Voice Agent ở quy mô lớn)
- **Diễn giả:** Trung Vu, Nghi Danh, Kiet Tran
- **Bản chất của Voice Agent:** Tác nhân giọng nói đòi hỏi giao tiếp đồng thời, 2 chiều (bidirectional audio) chứ không chỉ Request/Response thông thường.
- **Từ Demo đến Production:** Nhóm chọn kiến trúc *Cascaded Pipeline (STT -> LLM -> TTS)* thay vì *Speech-to-speech* vì: cần văn bản để kiểm duyệt (Reliability), cần gọi hàm chính xác (Tool calling), và xử lý tiếng Việt phức tạp tốt hơn.
- **Tối ưu hóa độ trễ:** Áp dụng kỹ thuật truyền dữ liệu liên tục (streaming), phản hồi đón đầu (Preemptive generation) và "làm nóng" (warm up) ngay khi bắt máy để giảm độ trễ tối đa.
- **Biết khi nào nên nói (Turn-taking):** Xây dựng mô hình hội thoại chuyên biệt cho tiếng Việt (độ chính xác 81%) để bot nhận biết người dùng đã nói xong, tránh ngắt lời vô duyên.
- **Kiểm soát hành vi:** Quản lý luồng bằng State Machine, quản lý phiên bản nghiêm ngặt và dùng RAG để đảm bảo bot chỉ trả lời dựa trên tài liệu ngân hàng (chống hallucination).
- **Đưa vào vận hành (Run the phones):** Đánh giá khắt khe bằng tự động hóa và Human-in-the-loop. Giám sát chi tiết mọi tương tác và tích hợp sâu với tổng đài (SIP, WebRTC, PII masking).

#### 3. AWS DevOps Agent: Your Always-Available Operations Teammate (AWS DevOps Agent: Thành viên vận hành luôn sẵn sàng trong đội ngũ của bạn)
- **Diễn giả:** Nguyen Nguyen, Bao Phan
- **Thách thức:** Quá trình điều tra sự cố thủ công vấp phải dữ liệu phân mảnh và thiếu hụt kiến thức, làm tăng cao MTTD và MTTR, khiến đội ngũ luôn bị động (Reactive).
- **Giải pháp AWS DevOps Agent:** Trợ lý AI tự động giúp giải quyết và ngăn chặn chủ động sự cố trên cả AWS, Azure và On-prem. Hỗ trợ phản hồi theo sự kiện, ngăn ngừa lỗi và thực hiện tác vụ theo yêu cầu.
- **Điểm khác biệt:** Học hỏi từ cấu trúc ứng dụng (Topology), tích hợp bảo mật qua Guardrail và MCP, tương tác liền mạch qua Slack/ServiceNow, thiết lập không cần hạ tầng (Zero-provision).
- **Cơ chế hoạt động (Incident Lifecycle):** Xử lý 4 bước: Sàng lọc và đối chiếu (Triage) -> Phân tích và suy luận (Investigation) -> Lập kế hoạch khắc phục (Mitigation) -> Báo cáo và phòng ngừa (Prevention).
- **Thành tựu thực tế:** Giảm thời gian xử lý sự cố đáng kể (WGU giảm 77% MTTR, ZENCHEF giảm 75% thời gian xử lý).

#### 4. AI-Powered Productivity: Workforce Planning For Enterprise (Năng suất hỗ trợ bởi AI: Quy hoạch nhân sự cho doanh nghiệp)
- **Diễn giả:** Truong Tran, Anh Dang
- **Thách thức nhân sự:** Sàng lọc CV thủ công tốn thời gian, tuyển dụng cảm tính làm tăng tỷ lệ thất bại, gây chậm trễ dự án và mất lợi thế cạnh tranh.
- **Giải pháp AI (Amazon Quick Suite):** Ứng dụng trợ lý ảo giúp giảm 80% thời gian lọc CV, hỗ trợ đưa ra quyết định dựa trên dữ liệu (data-driven) và tiết kiệm chi phí lớn cho doanh nghiệp.
- **Hệ sinh thái Amazon Quick:** Bao gồm Chat Agents, Research, Quick Sight, Flows (No-code) và Automate. Mọi ứng dụng đều được bảo vệ bởi các lớp bảo mật (Guardrails).
- **Kết nối dữ liệu:** Tích hợp đa nguồn (Relational Data Stores, SaaS như Jira/Workday, Knowledge Bases) thông qua engine siêu tốc SPICE.
- **Kịch bản thực tế 5 bước (Workforce Planning):** 
  1. *Connect:* Liên kết dữ liệu ứng viên.
  2. *Automate:* AI tự đánh giá điểm và gợi ý lương.
  3. *Visualize:* Vẽ dashboard phễu tuyển dụng.
  4. *Decide & Action:* Cập nhật trạng thái và sinh thư mời (Offer).
  5. *Track:* Tự động đặt lịch phỏng vấn.

#### 5. Building secure private MCP for Quick (Xây dựng kết nối MCP riêng tư bảo mật với Amazon Quick)
- **Diễn giả:** Toan Nguyen, Nghi Danh
- **Kiến trúc MCP cơ bản:** Khái quát về Model Context Protocol kết nối Host/Client (như Amazon Quick) tới các MCP Server để truy xuất dữ liệu hoặc API.
- **Thách thức bảo mật:** Mặc định trình kết nối MCP của Amazon Quick đi qua Internet (Public Endpoint), làm tăng bề mặt tấn công và vi phạm chính sách doanh nghiệp (Zero Trust).
- **Giải pháp VPC Connection:** Ép luồng dữ liệu của Amazon Quick đi qua card mạng nội bộ (Private-IP ENI) và phân giải tên miền bằng Route 53 Resolver (Private DNS).
- **Luồng xử lý khép kín (Request Flow):** Request đi từ Amazon Quick -> VPC Connection -> HTTPS tới Internal ALB (TLS termination) -> HTTP tới MCP Server. Đảm bảo luồng dữ liệu 100% riêng tư, tuyệt đối không đi ra Internet.

---

### Những Gì Học Được

*Sau buổi event em nghĩ là mình đã học được thêm kiến thức về Amazon Quick, MCP và cách MCP hoạt động, các đề tài khác em vẫn chưa hiểu và học được nhiều, có lẽ em sẽ tìm hiểu thêm về những đề tài còn lại sau, ngoài ra trong buổi event này em cũng đã tập được thói quen ghi chép lại, nó vừa giúp tránh buồn ngủ và tập trung lắng nghe hơn.*

---

### Ứng Dụng Vào Công Việc

*Có lẽ em sẽ tìm hiểu thêm về Amazon Quick và ứng dụng nó vào các dự án sau này của em, về các đề tài như Voice Agent hay DevOps Agent, em sẽ tìm hiểu thêm và cân nhắc áp dụng nó vào các dự án cá nhân khác của em.*

---

### Trải nghiệm trong event

*Vì đây là buổi event thứ 3 của em, em đã làm quen được với không khí của event và khá là phấn khích với các bài chia sẻ của các diễn giả, tuy nhiên buổi event lần này không được sôi động bằng 2 buổi event trước mà em đã tham gia.*

> *Buổi event lần này đối với em thấy diễn ra khá nhanh, nhưng dễ hiểu và dễ áp dụng hơn, ngoài ra thì em cũng không có nhận xét gì thêm với event lần này.*

---

#### Một số hình ảnh khi tham gia sự kiện

![Thòng Hoài Quý tham gia sự kiện FCAJ Community Day](/images/4-EventParticipated/event3_proof.jpg)

![Slide "How DevOps Agent work" giới thiệu vòng đời sự cố và cách DevOps Agent hoạt động](/images/4-EventParticipated/event3_slide1.jpg)

![Slide "Challenges: The Cost of Manual Incident Investigation" nói về các thách thức vận hành thủ công](/images/4-EventParticipated/event3_slide2.jpg)
