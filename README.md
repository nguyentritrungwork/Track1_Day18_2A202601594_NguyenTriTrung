# Track 1 - Day 18 — Designing and Testing Prototypes

## 1. Thông tin cá nhân và nhóm

- **MHV:** 2A202601594
- **Họ tên:** Nguyễn Trí Trung
- **Tên nhóm:** Nhóm 3 — E403
- **Thành viên nhóm:**
  1. Phạm Tiến Đại — 2A202601610
  2. Nguyễn Trí Trung — 2A202601594
  3. Tạ Thị Thu Huyền — 2A202601782
  4. Đỗ Thu Liễu —
- **Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher

---

## 2. Hypothesis Problem (Bản nhóm dùng trong Day 18)

> **Phát biểu Giả thuyết:**  
> Khi gặp các khái niệm khó hiểu hoặc trả lời sai trong lúc học lý thuyết/làm bài, học viên khóa học ngắn hạn gặp khó khăn trong việc tự xác định và lấp đầy chính xác lỗ hổng kiến thức nền đang thiếu vì thiếu công cụ giải đáp/chẩn đoán nhanh chóng, đáng tin cậy tại chỗ, dẫn đến việc phải dùng các workaround bên ngoài (AI ngoài, hỏi bạn bè) làm đứt mạch học, hoặc đối phó chọn bừa/bỏ qua kiến thức khiến lỗ hổng bị tích tụ lâu dài.

### Tính liên tục của Evidence (Gate 1 - Evidence Continuity)
Giả thuyết này được xây dựng và kế thừa trực tiếp từ các quan sát thực tế trong cuộc phỏng vấn ở Day 17:
* **Nối với Observation thực tế:** Học viên Hoàng Thiết Lâm trong buổi phỏng vấn ngày 17/8/2026 thừa nhận khi giảng viên giảng nhanh trên lớp, anh bị trôi mất 2-3 phần/buổi học và không biết hỏi ai hay xem lại thế nào khi tự học trước. Workaround của Lâm là dùng ChatGPT/Claude hoặc hỏi bạn xung quanh ngay tại lớp để được giải đáp tức thì (đáp ứng 80% nhu cầu). Khi về nhà, Lâm hầu như không tự ôn tập lại các phần bị lỡ vì không có cơ chế lưu trữ tự động.
* **Điều vẫn chưa biết (Unknowns):** Nhóm vẫn chưa chứng minh được liệu học viên có sẵn sàng từ bỏ thói quen dùng AI bên ngoài (ChatGPT, Claude) và bạn bè để tin dùng một nút bấm AI nội bộ mới hay không, và liệu việc chẩn đoán có làm họ cảm thấy mất kiên nhẫn khi đang kẹt bài tập.

---

## 3. Ba phương án giải pháp (Three Solution Options)

Chi tiết thiết kế của cả 3 option được trình bày tại: [three-option-design-sheet.md](file:///d:/Track1_Day18_2A202601594_NguyenTriTrung/three-option-design-sheet.md)

* **Option A: System-Led Diagnostic (AI-Driven)**
  * *Mô tả:* Hệ thống chủ động dẫn dắt luồng học bằng cách đặt 2-3 câu hỏi trắc nghiệm chẩn đoán nhanh để tìm ra khái niệm nền bị hổng, sau đó hiển thị bài ôn tập (Refresher) trực quan.
  * *Link Prototype:* [Figma Link Option A - AI-Driven Diagnostic](https://www.figma.com/proto/track1-day18-group3/option-a-system-led)
* **Option B: User-Led Concept Selection (Cooperative)**
  * *Mô tả:* Hệ thống đưa ra menu gợi ý 3-4 khái niệm nền liên quan. Học viên tự chọn khái niệm mình muốn ôn tập và làm bài tập tương tác (lật thẻ bài) để kiểm tra.
  * *Link Prototype:* [Figma Link Option B - Concept Selection](https://www.figma.com/proto/track1-day18-group3/option-b-concept-selection)
* **Option C: Context-Aware Chatbot Panel (Conversational)**
  * *Mô tả:* Một thanh chat trượt ra bên cạnh bài học. Học viên có thể tự do gõ câu hỏi hoặc bấm các prompt gợi ý nhanh để tương tác với AI Tutor.
  * *Link Prototype:* [Figma Link Option C - Conversational Chat](https://www.figma.com/proto/track1-day18-group3/option-c-conversational-chat)

Tất cả các link và kịch bản nhiệm vụ kiểm thử chung được lưu tại: [prototype-link.md](file:///d:/Track1_Day18_2A202601594_NguyenTriTrung/prototype-link.md)

---

## 4. Đóng góp của tôi trong nhóm (My Contribution)

Trong buổi làm việc nhóm Day 18, tôi (Nguyễn Trí Trung) đã trực tiếp đảm nhiệm các công việc sau:
1. **Thiết kế Option A (System-Led Diagnostic):** Trực tiếp thiết kế luồng tương tác và vẽ wireframe/prototype cho Option A, đảm bảo tích hợp nút thoát hiểm, hiển thị chỉ số không chắc chắn của AI để tăng tính kiểm soát của con người (Human Control).
2. **Chuẩn bị Kịch bản & Tổ chức Kiểm thử:** Thiết lập nhiệm vụ kiểm thử tiêu chuẩn (Standard Test Task) về "Nested For Loops" để đảm bảo tính độc lập và sẵn sàng kiểm thử của cả 3 option (Gate 4).
3. **Điều phối Thử nghiệm (Facilitation & Observation):** Trực tiếp chạy phiên thử nghiệm Option A với tester Đỗ Minh Quân, ghi lại biên bản kiểm thử chi tiết tại [prototype-feedback-note.md](file:///d:/Track1_Day18_2A202601594_NguyenTriTrung/prototype-feedback-note.md).
4. **Tổng hợp phản hồi nhóm (Synthesis):** Chủ trì buổi họp nhóm để đối chiếu ghi chép từ 3 phiên kiểm thử, tìm ra điểm chung/khác biệt và viết bản tổng hợp phản hồi tại [group-feedback-synthesis.md](file:///d:/Track1_Day18_2A202601594_NguyenTriTrung/group-feedback-synthesis.md).

---

## 5. Kết quả thử nghiệm Prototype (Prototype Feedback)

Tổng hợp chi tiết kết quả thử nghiệm được lưu trữ tại: [group-feedback-synthesis.md](file:///d:/Track1_Day18_2A202601594_NguyenTriTrung/group-feedback-synthesis.md)

* **Quan sát từ phiên tôi facilitate (Tester Đỗ Minh Quân - Option A):**
  * Quân hoàn thành nhiệm vụ sửa code thành công nhờ sơ đồ giải thích trực quan của Refresher.
  * Quân có cảm giác bị "ép buộc" làm quiz khi đang vội và đề xuất làm nổi bật nút bỏ qua chẩn đoán ("Xem giải thích trực tiếp").
* **Tổng hợp phản hồi 3 phiên (3-Tester Synthesis):**
  * *Điểm chung:* Cả 3 tester đều đánh giá cao tính trực quan của phần giải thích (sơ đồ, hình ảnh lật thẻ) và sự tiện lợi khi được hỗ trợ "tại chỗ" (in-context).
  * *Khác biệt:* Option A tìm đúng bệnh nhưng gây ức chế ngắn hạn; Option B thoải mái hơn nhưng học viên dễ chọn sai lỗ hổng thực tế; Option C linh hoạt nhưng dễ làm loãng thông tin do phản hồi của AI chatbot quá dài.
* **Next Change (Định hướng cải tiến):** Kết hợp cả 3 option thành luồng Hybrid: Khi bấm nút trợ giúp, hiển thị menu chọn khái niệm trước (Option B), đi kèm lựa chọn "Chẩn đoán tự động bằng quiz nhanh" (Option A). Refresher hiển thị dưới dạng sơ đồ trực quan kết hợp flashcard tương tác. Đồng thời, cải tiến nút "Bỏ qua chẩn đoán" trong Option A to rõ hơn để tăng tính kiểm soát.
* **Still Unproven (Điều chưa chứng minh được):** Liệu học viên có duy trì thói quen bấm nút này lâu dài hay không, và liệu việc gỡ kẹt liên tục tại chỗ có làm học viên lười tự tư duy sâu về sau.

---

## 6. Nhật ký hỗ trợ của AI (AI Support Log)

Chi tiết nhật ký tương tác và các quyết định Human-AI được ghi nhận tại: [ai-support-log.md](file:///d:/Track1_Day18_2A202601594_NguyenTriTrung/ai-support-log.md)

* **AI đã giúp:** Khởi tạo cấu trúc các file, phác thảo sự khác biệt cơ chế của 3 option và định hình văn phong các tài liệu tổng hợp phản hồi.
* **Sai sót/Hời hợt của AI:** AI đề xuất 3 option quá giống nhau về cơ chế (chỉ khác layout/nút bấm) và bỏ qua các yếu tố chi tiết về Human Control (Gate 2 & 3).
* **Tôi tự sửa:** Yêu cầu AI đổi 3 option thành 3 cơ chế riêng biệt (System-led vs. Selection vs. Chat sidebar), bổ sung nút skip chẩn đoán to rõ cho Option A, hiển thị mức độ tin cậy để biểu thị Uncertainty, và giới hạn kịch bản kiểm thử vào một lỗi code vòng lặp cụ thể (Gate 4).
