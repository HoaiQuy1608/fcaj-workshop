---
title: "FCAJ Community Day"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---



### Mục Đích Của Sự Kiện

- Chia sẻ kiến thức về vai trò của ngữ cảnh (context) trong việc ứng dụng AI hiệu quả.
- Giới thiệu trợ lý AI thông minh Amazon Quick và các tính năng hỗ trợ phân tích dữ liệu, tự động hóa quy trình.
- Giới thiệu các giải pháp bảo mật, tối ưu chi phí và nâng cao hiệu suất hạ tầng với Amazon CloudFront.
- Chia sẻ kinh nghiệm thực chiến từ cuộc thi Hackathon (LotusHacks) để xây dựng sản phẩm từ ý tưởng đến thực tế.
- Giải mã tính chất phi định tính (Non-Determinism) của các thiết lập LLM và cách giảm thiểu.
- Giới thiệu kiến trúc Multi-Agent cấp doanh nghiệp thông qua trường hợp chấm điểm tín dụng Startup.

### Danh Sách Diễn Giả

- **Vy Lam** - Senior Business Systems Analyst, VPBank
- **Thao Nguyen** - GenAI Engineer, VIB
- **Mai Nguyen** - GenAI Engineer, VIB
- **Uyen Le** - GenAI Engineer, VIB
- **Pham Nguyen Hai Anh** - Cloud Consultant, G-AsiaPacific Vietnam
- **Thinh Nguyen** - Devops Engineer, FCAJ
- **Tinh Truong** - Platform Engineer, GoTymeX
- **Duc Dao** - Solutions Architect, Cloud Kinetics

### Nội Dung Nổi Bật

#### 1. Context Is Everything: Making AI Actually Work for You (Ngữ cảnh là tất cả: Cách làm cho AI thực sự hoạt động hiệu quả)

- **Diễn giả:** Tinh Truong
- **Vấn đề cốt lõi của AI hiện tại:** Các mô hình AI hiện nay vốn đã rất mạnh mẽ, tuy nhiên lý do khiến chúng ta nhận lại những câu trả lời vô thưởng vô phạt hoặc sai hướng không phải do model kém, mà do thiếu "Ngữ cảnh" (Context). AI không thể tự động "đọc tâm trí" người dùng.
- **3 Sai lầm phổ biến khi Prompt:**
  - *The "Internet Puller":* Nhồi nhét quá nhiều tài liệu rác, không liên quan làm AI bị nhiễu thông tin (Chất lượng ngữ cảnh > Số lượng ngữ cảnh).
  - *Telling AI what it already knows:* Cung cấp những thông tin dư thừa mà AI đã biết thay vì tập trung vào những yêu cầu thay đổi tiếp theo.
  - *No Goal, No Constraints:* Đặt câu hỏi quá chung chung mà không có mục tiêu, rào cản hay tiêu chí thành công rõ ràng.
- **Tiến trình phát triển - Second AI Brain:** Tương lai của AI không chỉ nằm ở Prompt, mà là sự kết hợp giữa **Prompt + Context + Memory**. Khái niệm "Second AI Brain" (Bộ não AI thứ hai) ra đời giúp hệ thống tự động ghi nhớ, lưu trữ và truy xuất đúng ngữ cảnh cần thiết qua kiến trúc Vector DB.
- **Khung giao tiếp hiệu quả (Context Framework):** Luôn tuân thủ 4 yếu tố trước khi đặt câu hỏi cho AI: Xác định mục tiêu (Goal), Thông tin liên quan (Relevant info), Rào cản/Giới hạn (Constraints), và Tiêu chí thành công (Success criteria).

#### 2. Friendly AI Assistant with Amazon Quick (Trợ lý AI thân thiện với Amazon Quick)

- **Diễn giả:** Pham Nguyen Hai Anh
- **Giải quyết bài toán doanh nghiệp:** Người dùng doanh nghiệp thường phải lặp đi lặp lại những công việc tốn thời gian như tổng hợp thông tin, phân tích dữ liệu từ nhiều nguồn khác nhau.
- **Hệ sinh thái Amazon Q (Quick Suite):** Cung cấp trải nghiệm hợp nhất và an toàn với các khả năng Agentic AI mạnh mẽ, kết nối hơn 40 nguồn dữ liệu (Databases, Web search, User files) trong doanh nghiệp.
- **Tính năng nổi bật:**
  - *Quick Chat & Insights:* Hỏi đáp và truy xuất thông tin từ kho tàng tri thức (World knowledge & Company data).
  - *Quick Flows:* Tự động hóa các quy trình làm việc (Marketing, Sales, HR) mà không cần code.
  - *Quick Spaces & BI Dashboards:* Không gian cộng tác và trực quan hóa dữ liệu thông minh.
- **Ứng dụng thực tế (PM Assistant):** Trợ lý Quản lý dự án (PM) có thể tự động tạo biên bản cuộc họp (MoM), gửi email cho các bên liên quan và lên lịch cuộc họp tiếp theo chỉ bằng các thao tác cấu hình đơn giản.

#### 3. From Edge To Origin: CloudFront as Your Foundation (Từ Rìa đến Nguồn: CloudFront làm nền tảng)

- **Diễn giả:** Thinh Nguyen
- **Thách thức của khách hàng:** Khó kiểm soát và dự báo chi phí CDN do biến động traffic (tính phí pay-as-you-go). Người dùng thường lo sợ hóa đơn tăng đột biến do bị tấn công DDoS hoặc nội dung viral đột xuất.
- **Bảo vệ toàn diện (DDoS & Security):** 
  - Mạng lưới toàn cầu rộng lớn (700+ PoPs) phân tán và "hấp thụ" các cuộc tấn công DDoS khổng lồ ngay từ rìa mạng.
  - Tích hợp các tính năng nâng cao như Origin cloaking (ẩn máy chủ gốc qua OAC, VPC Origin), Viewer access control (Geo-blocking) và Signed URLs để chống ăn cắp nội dung.
- **Tối ưu hiệu suất & Chi phí:**
  - Cơ chế Multi-layer caching và Origin Shield giúp tăng Cache Hit Ratio, tránh sập nguồn.
  - Hỗ trợ HTTP/3 (QUIC/UDP) và tính năng nén tự động giúp giảm đến 81% thời gian tải.
  - Giảm tải đáng kể cho Load Balancer và CPU của máy chủ gốc (EC2 origin CPU giảm từ 5% xuống 1%). Nhờ đó, CloudFront thực chất lại là công cụ giúp cắt giảm tổng chi phí hạ tầng mạng.

#### 4. 36 hrs with LotusHacks – Building UTMorpho from Idea to Reality (36 giờ với LotusHacks – Xây dựng UTMorpho từ ý tưởng đến thực tế)

- **Diễn giả:** Thao Nguyen, Mai Nguyen, Uyen Le
- **Hành trình LotusHacks 2026:** Trải nghiệm thực tế 36 giờ code liên tục tại cuộc thi Hackathon lớn nhất Việt Nam.
- **Từ con số 0 đến UTMorpho:** Quá trình brainstorm ban đầu rất mông lung. Đội ngũ đã tìm thấy ý tưởng từ chính những rắc rối trong công việc hàng ngày (Look at daily work) để hình thành nên sản phẩm UTMorpho.
- **Thách thức kỹ thuật & Áp lực:** 
  - Phải đối mặt với các vấn đề AI sinh ra quá nhiều dữ liệu rác (AI Overgeneration), giới hạn Token (Token limits), và sự kiệt sức khi gần đến giờ thuyết trình (Burnout).
  - Bước ngoặt (Turning point) là khi nhóm tập trung vào "Focused Editing Experience", cắt bỏ tính năng rườm rà để làm nổi bật giá trị cốt lõi.
- **Bài học kinh nghiệm:** Những sự ức chế và bất cập trong thực tế (Real Frustration) mới là thứ tạo ra ý tưởng tốt. "Nhiều ý tưởng hơn không có nghĩa là ý tưởng tốt hơn". Và cuối cùng, sự đồng bộ trong team (Team Sync) là yếu tố quyết định sống còn.

#### 5. Non-Determinism of "Deterministic" LLM Settings (Tính phi định tính của các thiết lập LLM "định tính")

- **Diễn giả:** Duc Dao
- **Lầm tưởng về Temperature = 0:** Rất nhiều kỹ sư cho rằng cài đặt `Temperature = 0` sẽ khiến LLM trở thành một cỗ máy "định tính" tuyệt đối (đầu vào giống nhau luôn cho ra đầu ra y hệt). Điều này được tin dùng cho việc ép kiểu JSON hoặc Automated Testing.
- **Sự thật phũ phàng (The Reality):** Các nghiên cứu chỉ ra rằng độ chính xác có thể chênh lệch lên đến 15% (thậm chí 70% trên cùng 1 tác vụ) giữa các lần chạy giống hệt nhau.
- **Nguyên nhân cốt lõi:**
  - *Kỹ thuật (Technical):* Phép toán dấu phẩy động trên GPU chạy song song không có tính kết hợp `(a+b)+c != a+(b+c)`. Sai số siêu nhỏ này có thể làm thay đổi kết quả chọn token cuối cùng.
  - *Thương mại (Commercial):* Do cơ chế "Inference batching". Các API Provider gộp nhiều request của nhiều người dùng vào chung một batch để tiết kiệm tài nguyên GPU, vô tình làm thay đổi luồng tính toán.
- **Chiến lược giảm thiểu:** 
  - Nên thiết kế hệ thống chấp nhận sự sai lệch (Build with variance in mind).
  - Nên sử dụng `Temp = 0.1` thay vì `0` để tránh việc model bị kẹt trong vòng lặp vô tận (repetitive loops).

#### 6. Enterprise-Grade Multi-Agent System: The Case of Startup Credit Scoring (Hệ thống Multi-Agent cấp doanh nghiệp: Trường hợp chấm điểm tín dụng Startup)

- **Diễn giả:** Vy Lam
- **Sự lệch pha dữ liệu:** Các hệ thống chấm điểm tín dụng ngân hàng truyền thống (đòi hỏi 3 năm BCTC, tài sản thế chấp) hoàn toàn thất bại khi áp dụng cho Startups (vốn chỉ có 6-18 tháng hoạt động, tài sản là IP và Team).
- **Điểm yếu của Single Agent:** Việc dùng 1 Agent duy nhất đóng vai trò "Người phê duyệt" sẽ gây quá tải ngữ cảnh, pha loãng chuyên môn, thiếu cơ chế kiểm tra chéo và dễ tạo ra điểm mù (Single point of failure).
- **Kiến trúc Multi-Agent (Hội đồng tín dụng ảo):** Xây dựng một "Virtual credit committee" với nhiều Agent chuyên biệt: Financial Analyst, Market Analyst, Team Evaluator, Risk Assessor và Compliance.
  - *Lợi ích:* Xử lý song song, lưu vết rõ ràng (Auditability), và có sự phản biện chéo giữa các Agent.
- **Tiêu chuẩn cấp doanh nghiệp (Enterprise-Grade):** Để lên Production, hệ thống phải đáp ứng 6 trụ cột: Security (MFA, Encryption), Data Governance, Network (VPC, Private endpoints), Operations, Human Factors, và Compliance (SOC 2, GDPR).
- **Lợi ích vận hành (ROI):** Tốc độ xử lý hồ sơ giảm 95% (từ 2-3 tuần xuống 2-4 giờ), tiết kiệm 95% chi phí. AI Doanh nghiệp không chỉ là "làm cho nó chạy được", mà phải là "chạy an toàn, đáng tin cậy và có khả năng mở rộng".

---

### Những Gì Học Được

*Sau buổi event, em học được rất nhiều điều bổ ích đến từ anh chị, đặc biệt là kiến thức về cách tối ưu chi phí với CloudFront và cách quản lý thời gian, phân bổ thời gian hợp lý khi làm việc nhóm, và nhiều điều bổ ích khác.*

---

### Ứng Dụng Vào Công Việc

*Về việc ứng dụng các kiến thức mà em đã nghe, em nghĩ là em có thể ứng dụng được cách quản lý thời gian, phân bổ thời gian, công việc hợp lý khi làm việc nhóm và có thể tối ưu chi phí khi sử dụng CloudFront. Các kiến thức còn lại khá mới mẻ đối với em, vì vậy có lẽ em sẽ tìm hiểu và vận dụng trong thời gian tới.*

---

### Trải nghiệm trong event

*Khi tham gia event FCAJ Community Day hôm nay, em cảm thấy rất hào hứng và vui khi được nghe các anh chị chia sẻ về các kiến thức thực tế khi sử dụng AI để làm việc. Mặc dù vẫn còn hơi ngại và chưa dám đặt câu hỏi nhưng em cũng đã học hỏi được rất nhiều điều từ event, và em cũng đã có cơ hội tiếp xúc và trò chuyện với rất nhiều bạn tham gia khác. Mặc dù event này là lần thứ hai em tham gia nhưng em cảm giác như là lần đầu vậy, hồi hộp và mong chờ.*

---

#### Một số hình ảnh khi tham gia sự kiện

![Thòng Hoài Quý tham gia sự kiện FCAJ Community Day](/images/4-EventParticipated/event2_proof.jpg)

![Slide "Context Is Everything" trình bày bởi anh Tinh Truong](/images/4-EventParticipated/event2_slide1.jpg)

> *Cuối cùng, em thấy event hôm nay là một event cực kỳ bổ ích, event này giúp em biết được thêm nhiều kiến thức mới, và cũng có cơ hội để giao lưu với các bạn tham gia khác.*
