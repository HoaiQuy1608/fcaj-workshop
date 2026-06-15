---
title: "AWS First Cloud Journey - Workshop"
date: 2026-05-09
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

{{% notice warning %}}
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn kể cả warning này.
{{% /notice %}}

# Bài thu hoạch “AWS First Cloud Journey - [Tên Sự Kiện / Workshop]”

### Mục Đích Của Sự Kiện

- *(Nhập các mục tiêu chính của sự kiện tại đây)*
- *(Nhập các kiến thức hoặc công nghệ mà buổi workshop muốn chia sẻ tại đây)*

### Danh Sách Diễn Giả

- **Huỳnh Hoàng Long** - Admin of FCAJ
- **Nguyen Tuan Thinh** - DevOps/Cloud Engineer, First Cloud AI Journey
- **Khang** - Diễn giả bài chia sẻ 3
- **Thảo Nguyễn** - GenAI Engineer, VIB

### Nội Dung Nổi Bật

#### 1. Addicted to Learning Like You're Addicted to Social Media (Nghiện học như nghiện mạng xã hội)
- **Diễn giả:** Huỳnh Hoàng Long (Admin of FCAJ)
- **Nguyên lý Dopamine:** Dopamine giải phóng khi kỳ vọng nhận phần thưởng. Áp dụng "Phần thưởng biến thiên" (Variable Reward) và "Vòng lặp học tập" (Tò mò → Thử nghiệm → Khám phá → Thỏa mãn) để duy trì hứng thú.
- **3 thủ thuật não bộ giúp học tập như chơi game:**
  * *Sợ mất mát (Fear of Loss):* Duy trì học tập qua cơ chế chuỗi ngày liên tục (streak giống Duolingo, ngọn lửa TikTok, quà điểm danh game).
  * *Đánh lừa hạch hạnh nhân (Trick the Amygdala):* Đơn giản hóa mục tiêu bằng **Quy tắc 2 phút** (chỉ mở file, đọc 1 trang, giải 1 câu để dễ bắt đầu).
  * *Phản hồi tức thì (Create Instant Feedback):* Tự thưởng ngay sau khi hoàn thành mốc học tập (học 25 phút được +10 XP, xong 1 chương tự thưởng ly cafe).
- **Kết luận:** Người chiến thắng là người xây dựng được hệ thống thói quen giúp họ tự động tiếp tục mỗi ngày.

#### 2. Automated Prompt Engineering: Enhancing LLM Output Quality (Kỹ thuật Prompt tự động)
- **Diễn giả:** Nguyen Tuan Thinh (DevOps/Cloud Engineer, First Cloud AI Journey)
- **Tổng quan:** Viết prompt rõ ràng, có cấu trúc (Role, Instruction, Context, Constraints...) giúp tối ưu chất lượng đầu ra và chi phí token (Token Economics).
- **Kỹ thuật Prompt nâng cao (Advanced Techniques):**
  * *Chain-of-Thought (CoT) & Self-Consistency:* Suy luận theo chuỗi tuần tự và chọn đáp án có độ đồng thuận cao nhất.
  * *Tree of Thoughts (ToT):* Phân nhánh suy luận dạng cây để tìm phương án tối ưu.
  * *RAG & Role Prompting.*
- **Dự án Proptimizer (Kiến trúc giải pháp):** Tiện ích mở rộng trình duyệt giúp tự động tối ưu hóa prompt và chat với AI:
  * *S3 & CloudFront:* Lưu trữ và phân phối trang tĩnh với độ trễ thấp toàn cầu.
  * *Cognito:* Đăng ký, đăng nhập và xác thực người dùng bảo mật qua token JWT.
  * *API Gateway & Lambda:* Định tuyến API và xử lý logic nghiệp vụ serverless.
  * *Amazon Bedrock:* Tích hợp các mô hình nền tảng (như Claude) để tối ưu prompt.
  * *DynamoDB & CloudWatch:* Lưu trữ dữ liệu hệ thống (NoSQL) và giám sát hiệu năng/logs.
  * *Chi phí & Demo:* Tối ưu chi phí hạ tầng ở mức 0 USD (chưa tính Bedrock). Trang web demo được chạy tại `https://d3jqm7so635aqb.cloudfront.net`.

#### 3. AI-Ready Freshers: Skills and Mindset in the AI Era (Trang bị tư duy trong kỷ nguyên AI)
- **Diễn giả:** Khang
- **Tác động của AI & Hệ số nhân:** AI là hệ số nhân (multiplier), có thể nâng cao hoặc hạ thấp năng lực của bạn. Bạn có thể thuê ngoài tư duy (outsource thinking) nhưng không thể thuê ngoài sự thấu hiểu (outsource understanding).
- **Tư duy cầu tiến (Growth Mindset) & Sự chính trực (Integrity):**
  * Tò mò hỏi "Tại sao", đón nhận lỗi sai làm bài học.
  * Làm tốt nhất ngay cả khi không có ai giám sát, không lạm dụng "đường tắt" AI mà tập trung vào phẩm chất bản thân.
- **Định hướng công việc & Tiêu chí đánh giá:**
  * Công việc lý tưởng là giao điểm của 3 vòng tròn: Việc bạn thích (Đam mê), Việc mang lại lợi ích (Quyền lợi) và Việc phải làm (Trách nhiệm).
  * 5 Lợi ích của công việc: Lương, Kinh nghiệm, Mạng lưới quan hệ, Kiến thức và Sự phát triển.
  * 5 Tiêu chí doanh nghiệp đánh giá: Thái độ (Attitude), Trình độ (Competence), Kinh nghiệm (Experience), Trải nghiệm (Exposure) và Tố chất (Potential).
- **Hành động tiếp theo (Next Actions):** Luôn đặt câu hỏi "Tại sao?" (tự giả định nếu chưa biết), lập lộ trình dài hạn (nhìn xa, bắt đầu từ việc nhỏ - *Look far, start Small*) và phát triển đội ngũ làm việc nhóm vì *"đi nhanh đi một mình, đi xa đi cùng team"*.

#### 4. BMAD Method: Đưa cả đội ngũ Agile & AI vào trong IDE của bạn (Phương pháp BMAD)
- **Diễn giả:** Thảo Nguyễn (GenAI Engineer, VIB)
- **Vấn đề của Vibe Coding:** Giao phó toàn bộ dự án cho một khung chat đơn nhất dễ dẫn đến phình to ngữ cảnh (Context Bloat), lỗi code chắp vá và bỏ qua quy trình phát triển phần mềm (SDLC).
- **Phương pháp BMAD (Context Engineering):** Chuyển dịch sang mô hình Agile với đội ngũ AI Agents chuyên biệt (Orchestrator, PM, Architect, PO, Scrum Master, Dev & Reviewer).
- **Quy trình khép kín:**
  * *Planning & Sharding:* Định hình PRD và Kiến trúc Tech Stack, sau đó phân mảnh tài liệu thành các chunks siêu nhỏ để tránh quá tải bộ nhớ và ảo giác của LLM.
  * *Execution & Testing:* Scrum Master phân bổ Story, Developer Agent tự động thực thi code và Review Agent chạy vòng lặp kiểm thử liên tục cho đến khi lỗi bằng 0.
- **Hệ sinh thái & Triển khai:** Hỗ trợ mở rộng qua các Module (BMAD Core, Creative Suite, BMB, TEA) và cài đặt cục bộ cực nhanh qua lệnh `npx bmad-method@next install .` (tích hợp Cursor, Windsurf, Claude Code). Mã nguồn mở tại `github.com/bmad-code-org/BMAD-METHOD`.

---

### Những Gì Học Được

*(Bạn tự điền nội dung các bài học rút ra của bản thân tại đây)*

---

### Ứng Dụng Vào Công Việc

*(Bạn tự điền kế hoạch ứng dụng kiến thức vào công việc/học tập của bản thân tại đây)*

---

### Trải nghiệm trong event

*(Bạn tự điền trải nghiệm và cảm xúc thực tế khi tham gia sự kiện tại đây)*

---

#### Một số hình ảnh khi tham gia sự kiện

*(Thêm các hình ảnh tham gia sự kiện của bạn tại đây)*

> *(Bạn tự điền nhận xét hoặc kết luận chung của bạn tại đây)*
