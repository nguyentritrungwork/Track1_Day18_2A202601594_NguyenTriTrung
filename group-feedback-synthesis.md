

**Case:** Case A — AI Tutor: Diagnostic Refresher  
**Nhóm:** Nhóm 3 — E403  

Tài liệu này tổng hợp kết quả thử nghiệm từ cả 3 phiên kiểm thử prototype của nhóm và đưa ra các định hướng cải tiến tiếp theo.

---

## 1. Tóm tắt 3 Phiên kiểm thử (Three Feedback Notes Summary)

### Phiên 1 (Nguyễn Trí Trung facilitate): Tester Đỗ Minh Quân thử nghiệm Option A (System-Led Diagnostic)
* **Hành vi & Phản ứng:** Quân loay hoay sửa code ma trận 1 phút trước khi bấm nút hỗ trợ. Anh bị khựng lại khi hệ thống yêu cầu làm 2 câu hỏi trắc nghiệm chẩn đoán (MCQ) và cảm thấy hơi căng thẳng/bực mình vì muốn câu trả lời ngay. Tuy nhiên, sau khi hoàn thành MCQ, anh đánh giá sơ đồ giải thích trực quan của Refresher cực kỳ hiệu quả, giúp anh tự nhận ra lỗi nhầm lẫn giữa chỉ mục `i` và `j`.
* **Mức độ kiểm soát:** Tìm thấy nút thoát hiểm "Quay lại bài" nhưng cho rằng nút bỏ qua quiz chẩn đoán ("Xem giải thích trực tiếp") thiết kế quá chìm, tạo cảm giác bị hệ thống bắt buộc.

### Phiên 2 (Phạm Tiến Đại facilitate): Tester Nguyễn Việt Hà thử nghiệm Option B (User-Led Concept Selection)
* **Hành vi & Phản ứng:** Hà bấm nút hỗ trợ ngay khi chạy thử code lỗi lần đầu tiên. Khi màn hình menu hiển thị 3 khái niệm nền, cô phân vân giữa "Vòng lặp For lồng nhau" và "Biến chỉ mục". Cô chọn "Biến chỉ mục" và đọc giải thích, sau đó làm hoạt động tương tác nhỏ (lật thẻ bài). Hà cảm thấy thích thú với hoạt động lật thẻ vì nó giúp cô củng cố lại lý thuyết một cách chủ động.
* **Mức độ kiểm soát:** Hà đánh giá cao việc cô được tự do lựa chọn chủ đề mình muốn học, nhưng cô cũng bối rối vì không chắc chắn 100% là mình chọn đúng lỗ hổng thực tế của bản thân.

### Phiên 3 (Tạ Thị Thu Huyền facilitate): Tester Trần Đăng Khoa thử nghiệm Option C (Conversational Chatbot)
* **Hành vi & Phản ứng:** Khoa bấm nút và thanh chat mở ra bên phải. Khoa không tự gõ câu hỏi mà click ngay vào câu gợi ý nhanh: "Giải thích cách chạy của i và j". AI phản hồi khá dài, Khoa phải cuộn thanh chat liên tục để đọc. Sau đó Khoa chat hỏi thêm một câu: "cho mình ví dụ code Python". AI phản hồi nhanh và hữu ích.
* **Mức độ kiểm soát:** Khoa cảm thấy thoải mái vì thanh chat nằm một bên, anh vẫn nhìn thấy code bài tập bên trái để đối chiếu. Anh thoát chat dễ dàng bằng cách bấm nút đóng, nhưng lịch sử chat thỉnh thoảng che mất một phần giao diện khiến anh phải kéo thả bảng chat thủ công.

---

## 2. So sánh và Phân tích Pattern/Khác biệt (Patterns & Differences)

### Các Pattern trùng lặp (Common Patterns):
* **Sự quan trọng của tính trực quan:** Cả 3 tester đều đánh giá cao các nội dung giải thích có đi kèm sơ đồ, ví dụ minh họa trực quan hoặc định dạng dễ đọc (sơ đồ ở Option A, lật thẻ ở Option B, code block ở Option C).
* **Nhu cầu không đứt mạch (No flow-breaking):** Học viên đều đánh giá cao việc họ không phải mở Google hay rời khỏi bài học để tra cứu. Cảm giác được hỗ trợ "tại chỗ" (in-context) làm họ tự tin hơn.

### Các điểm khác biệt lớn (Key Differences):
* **Cảm xúc đối với chẩn đoán tự động (Option A) vs. Tự lựa chọn (Option B):** 
  * Option A giúp tìm đúng bệnh nhưng gây ức chế ngắn hạn vì học viên phải giải câu đố khi đang căng thẳng. 
  * Option B tạo cảm giác dễ chịu, chủ động hơn nhưng lại đặt gánh nặng tự đánh giá lên vai học viên (những người có thể không biết mình đang sai ở đâu).
* **Hiệu suất đọc hiểu:** Thanh chat (Option C) phản hồi linh hoạt nhưng văn bản quá dài làm học viên lười đọc. Trong khi đó, các câu hỏi chẩn đoán (Option A) và hoạt động tương tác lật thẻ (Option B) giúp định hướng sự tập trung tốt hơn.

---

## 3. Định hướng cải tiến tiếp theo (Next Change)

Nhóm quyết định kết hợp ưu điểm của cả 3 option để tạo ra một thiết kế cải tiến (Hybrid Design):
1. **Thiết kế lại Cơ chế Chẩn đoán (Hybrid Diagnostic):** Khi bấm nút "Tôi vẫn chưa hiểu", hệ thống sẽ hiển thị Menu lựa chọn các khái niệm nền (như Option B) để học viên tự chọn nếu họ tự tin. Tuy nhiên, hệ thống sẽ chèn thêm một lựa chọn nổi bật: **"Chẩn đoán tự động bằng AI (2 câu hỏi nhanh)"** dành cho những học viên hoàn toàn bế tắc và không biết mình thiếu gì (đáp ứng Note 1 và Note 2).
2. **Cải tiến Trực quan & Tương tác:** Refresher của tất cả các khái niệm sẽ sử dụng sơ đồ luồng chạy trực quan thay vì chỉ dùng văn bản dài, kết hợp hoạt động lật thẻ (Flashcard) tương tác nhẹ để học viên tự kiểm tra kiến thức trước khi quay về làm bài.
3. **Tối ưu hóa Quyền kiểm soát (Enhanced Human Control):** Nút "Xem giải thích trực tiếp (Bỏ qua chẩn đoán)" trong luồng chẩn đoán tự động sẽ được làm to rõ ràng, đặt cạnh nút chọn đáp án để học viên có thể thoát luồng trắc nghiệm bất cứ khi nào họ cảm thấy mất kiên nhẫn.

---

## 4. Điều vẫn chưa được chứng minh (Still Unproven)

* **Tần suất sử dụng thực tế:** Liệu học viên có duy trì thói quen bấm nút hỗ trợ này trong suốt khóa học dài ngày hay không, hay họ sẽ chỉ bấm thử vài lần đầu vì tò mò rồi quay lại thói quen cũ là tra Google/hỏi bạn bè.
* **Tác động lâu dài đến học tập:** Việc AI Tutor gỡ kẹt liên tục ngay tại chỗ có khiến học viên trở nên lười tự tư duy sâu, hay nó thực sự giúp họ xây dựng nền tảng vững chắc để tự giải quyết các bài tập khó hơn về sau.
