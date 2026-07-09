---
title: "FCAJ Community Day"
date: 2026-05-09
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Bài thu hoạch “AWS First Cloud Journey - FCAJ Community Day”

### Mục Đích Của Sự Kiện

- Tìm hiểu các chiến lược học tập thông qua trò chơi hóa (gamification) để xây dựng thói quen hiệu quả và duy trì chuỗi học tập liên tục.
- Học hỏi các kỹ thuật kỹ nghệ gợi ý (prompt engineering) từ cơ bản đến nâng cao nhằm tối ưu hóa chất lượng câu trả lời của các mô hình ngôn ngữ lớn (LLM).
- Tìm hiểu về kinh tế học token (token economics) và thiết kế kiến trúc serverless của ứng dụng tối ưu hóa prompt (Proptimizer) trên nền tảng đám mây AWS.
- Giới thiệu phương pháp BMAD (Agile & AI Agents) tích hợp trong môi trường phát triển (IDE) giúp tối ưu hóa quy trình làm việc nhóm và phát triển phần mềm.

### Danh Sách Diễn Giả

- **Huynh Hoang Long** - Admin of FCAJ
- **Nguyen Tuan Thinh** - DevOps/Cloud Engineer, First Cloud AI Journey
- **Khang** - Diễn giả bài chia sẻ 3
- **Thao Nguyen** - GenAI Engineer, VIB

### Nội Dung Nổi Bật

#### 1. Addicted to Learning Like You're Addicted to Social Media (Nghiện học như nghiện mạng xã hội)
- **Diễn giả:** Huynh Hoang Long (Admin of FCAJ)
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
- **Diễn giả:** Thao Nguyen (GenAI Engineer, VIB)
- **Vấn đề của Vibe Coding:** Giao phó toàn bộ dự án cho một khung chat đơn nhất dễ dẫn đến phình to ngữ cảnh (Context Bloat), lỗi code chắp vá và bỏ qua quy trình phát triển phần mềm (SDLC).
- **Phương pháp BMAD (Context Engineering):** Chuyển dịch sang mô hình Agile với đội ngũ AI Agents chuyên biệt (Orchestrator, PM, Architect, PO, Scrum Master, Dev & Reviewer).
- **Quy trình khép kín:**
  * *Planning & Sharding:* Định hình PRD và Kiến trúc Tech Stack, sau đó phân mảnh tài liệu thành các chunks siêu nhỏ để tránh quá tải bộ nhớ và ảo giác của LLM.
  * *Execution & Testing:* Scrum Master phân bổ Story, Developer Agent tự động thực thi code và Review Agent chạy vòng lặp kiểm thử liên tục cho đến khi lỗi bằng 0.
- **Hệ sinh thái & Triển khai:** Hỗ trợ mở rộng qua các Module (BMAD Core, Creative Suite, BMB, TEA) và cài đặt cục bộ cực nhanh qua lệnh `npx bmad-method@next install .` (tích hợp Cursor, Windsurf, Claude Code). Mã nguồn mở tại `github.com/bmad-code-org/BMAD-METHOD`.

---

### Những Gì Học Được

*Những gì em học được tại buổi event đầu tiên là về cách tự tạo động lực cho em để học tập hiệu quả hơn mặc dù em khá là lười biếng và thường dành thời gian cho game nhiều hơn nhưng sau khi nghe anh Long chia sẻ thì em nghĩ là em sẽ thử cách thêm phần thưởng sau khi học được một kiến thức mới nào đó. Ngoài ra em nghĩ phương thức BMAD cũng rất hay và em nghĩ nó sẽ có ích đối với nhiều người, giúp mọi người tiết kiệm thời gian và công sức trong việc phát triển phần mềm.*

---

### Ứng Dụng Vào Công Việc

*Về ứng dụng vào việc học hay công việc thì em thấy BMAD cũng rất hợp để em có thể ứng dụng nó để làm project cho bản thân, ngoài ra thì bài chia sẻ của anh Long cũng có thể áp dụng hiệu quả đối với việc học của em để giúp em nghiện học hơn là nghiện chơi game.*

--- 

### Trải nghiệm trong event

*Lần đầu tiên em tham gia event này em thấy khá là hồi hộp và lo lắng một chút vì em khá là ngại khi có nhiều người như thế này, nhưng sau khi trải nghiệm thì em nghĩ em muốn lên thêm nữa, mặc dù em chưa dám đứng lên để chia sẻ các kiến thức đến với mọi người nhưng em nghĩ tham gia và nghe cũng giúp ích cho bản thân nhiều hơn.*

---

> *Nhận xét của em về lần đầu tiên tham gia event này thì nó là một trải nghiệm tuyệt vời và đáng để tham gia, em mong có thể tham gia các event tiếp theo để được nghe thêm nhiều kiến thức và kinh nghiệm của các anh chị đi trước.*
