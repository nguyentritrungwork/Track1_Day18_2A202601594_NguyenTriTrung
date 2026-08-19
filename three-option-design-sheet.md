

**Case:** Case A — AI Tutor: Diagnostic Refresher  
**Nhóm:** Nhóm 3 — E403  
**Dự án:** AI Tutor hỗ trợ học viên vượt qua điểm nghẽn kiến thức  

Bản thiết kế này mô tả chi tiết 3 Option giải pháp khác nhau về mặt cơ chế (Mechanism) và cách phân chia nhiệm vụ giữa Người và AI (Human-AI Task Split) nhằm giải quyết cùng một Hypothesis Problem.

---

## 1. Option A: System-Led Diagnostic (AI-Driven)
*Cơ chế tự động chẩn đoán chủ động do hệ thống dẫn dắt.*

* **Cơ chế hoạt động:** Khi học viên bấm nút "Tôi vẫn chưa hiểu", AI Tutor sẽ chủ động nắm quyền kiểm soát luồng học. Dựa trên lịch sử trả lời sai gần đây và nội dung slide hiện tại, AI sẽ chọn ra 2 khái niệm nền nghi ngờ nhất, tạo ra 2-3 câu hỏi trắc nghiệm chẩn đoán ngắn (Diagnostic MCQ). Dựa vào câu trả lời của học viên, AI xác định chính xác lỗ hổng, hiển thị một đoạn giải thích ngắn kèm ví dụ và đưa học viên trở lại bài học.
* **Phân chia công việc giữa User và AI (Human-AI Split):**
  * **AI:** Phân tích ngữ cảnh, lựa chọn khái niệm chẩn đoán, tự động tạo câu hỏi trắc nghiệm, đánh giá kết quả, và soạn thảo Refresher.
  * **Học viên (User):** Trả lời các câu hỏi trắc nghiệm chẩn đoán và đọc phần giải thích được đề xuất.
* **Cơ chế kiểm soát của con người (Human Control):**
  * **Expectation (Kỳ vọng):** Học viên hiểu rằng hệ thống đang hỏi để chẩn đoán lỗ hổng, giúp họ không phải tự dò tìm. Hệ thống thông báo rõ: "Để giúp bạn hiểu bài, hãy trả lời nhanh 2 câu hỏi sau để mình tìm đúng chỗ bạn bị kẹt nhé."
  * **Agency (Khả năng can thiệp):** Học viên có thể bỏ qua chẩn đoán (nút "Xem giải thích trực tiếp") hoặc chọn xem danh sách các khái niệm liên quan thay vì làm trắc nghiệm.
  * **Evidence/Uncertainty (Tín hiệu không chắc chắn):** Hệ thống hiển thị mức độ nghi ngờ của AI (ví dụ: "Mình đoán bạn đang vướng ở '0-based Indexing' (90%) hoặc 'Loop Condition' (10%)").
  * **Recovery (Đường thoát hiểm):** Nút "Quay lại bài học" luôn xuất hiện ở góc màn hình để học viên thoát ra ngay lập tức nếu cảm thấy chẩn đoán bị sai hoặc phiền phức.

---

## 2. Option B: User-Led Concept Selection (Cooperative)
*Cơ chế hợp tác, AI đề xuất danh mục và học viên chủ động tự xác định lỗ hổng.*

* **Cơ chế hoạt động:** Khi bấm nút "Tôi vẫn chưa hiểu", hệ thống không tự chẩn đoán mà hiển thị một bảng chọn (Menu) chứa 3-4 khái niệm nền liên quan trực tiếp đến bài học hiện tại (do AI trích xuất và ánh xạ từ bài học). Học viên sẽ tự chọn khái niệm mình cảm thấy mơ hồ nhất. AI sau đó sẽ hiển thị một phần giải thích ngắn gọn đi kèm một hoạt động tương tác nhỏ (như lật thẻ hoặc điền vào chỗ trống) để học viên tự kiểm tra sự hiểu biết trước khi quay lại bài học.
* **Phân chia công việc giữa User và AI (Human-AI Split):**
  * **AI:** Quét nội dung bài học, ánh xạ các khái niệm nền liên quan, tạo Refresher động và hoạt động tương tác cho khái niệm học viên đã chọn.
  * **Học viên (User):** Tự đánh giá bản thân (Self-assessment) để lựa chọn đúng khái niệm mình cần ôn từ danh sách gợi ý.
* **Cơ chế kiểm soát của con người (Human Control):**
  * **Expectation (Kỳ vọng):** Học viên biết họ sẽ được cung cấp một danh mục khái niệm để tự lựa chọn. Hệ thống thông báo: "Dưới đây là các khái niệm nền cần thiết cho bài học này. Hãy chọn phần bạn muốn ôn lại nhé!"
  * **Agency (Khả năng can thiệp):** Học viên có toàn quyền lựa chọn khái niệm muốn xem, có thể chọn nhiều khái niệm cùng lúc hoặc chuyển đổi qua lại giữa các khái niệm.
  * **Evidence/Uncertainty (Tín hiệu không chắc chắn):** Mỗi khái niệm được đính kèm một câu mô tả ngắn về lý do tại sao nó lại quan trọng đối với bài học hiện tại (ví dụ: "Bạn cần khái niệm này để hiểu dòng code số 7").
  * **Recovery (Đường thoát hiểm):** Học viên có thể bấm "Đóng" để quay lại bài học chính hoặc bấm "Đổi khái niệm khác" để quay lại menu chọn ban đầu bất cứ lúc nào.

---

## 3. Option C: Context-Aware Chatbot Panel (Conversational)
*Cơ chế đối thoại tự do dưới dạng thanh chat bên cạnh bài học.*

* **Cơ chế hoạt động:** Khi bấm nút "Tôi vẫn chưa hiểu", một thanh chat (Side Panel) sẽ trượt ra từ bên phải màn hình, giữ nguyên nội dung bài học bên trái. AI Chatbot bắt đầu bằng một câu hỏi thân thiện: "Mình thấy bạn đang dừng ở Slide 'Vòng lặp For'. Bạn gặp khó khăn ở dòng code nào hoặc từ khóa nào?". Học viên có thể tự do nhập câu hỏi (Free-text prompt) hoặc click vào các câu hỏi gợi ý nhanh (Quick prompts) như "Giải thích dòng 3", "Ví dụ dễ hiểu hơn", hoặc "Dịch cú pháp này sang Python".
* **Phân chia công việc giữa User và AI (Human-AI Split):**
  * **AI:** Đóng vai trò là gia sư đàm thoại, phân tích ngữ cảnh bài học hiện tại và câu hỏi của học viên để đưa ra câu trả lời cá nhân hóa theo thời gian thực.
  * **Học viên (User):** Chủ động đặt câu hỏi hoặc định hướng cuộc hội thoại thông qua các prompt để lấy đúng thông tin mình cần.
* **Cơ chế kiểm soát của con người (Human Control):**
  * **Expectation (Kỳ vọng):** Học viên biết đây là không gian đối thoại tự do và riêng tư. AI bắt đầu bằng việc chào hỏi và đưa ra các gợi ý mẫu để hướng dẫn học viên cách bắt đầu.
  * **Agency (Khả năng can thiệp):** Học viên có thể gõ bất kỳ câu hỏi nào họ muốn, điều khiển chiều sâu giải thích của AI bằng cách yêu cầu "giải thích chi tiết hơn" hoặc "tóm tắt ngắn gọn".
  * **Evidence/Uncertainty (Tín hiệu không chắc chắn):** Khi trả lời, AI trích dẫn chính xác dòng code hoặc từ khóa trong bài học mà nó đang giải thích để học viên đối chiếu.
  * **Recovery (Đường thoát hiểm):** Một nút lớn "Đóng Chat & Học Tiếp" ở đầu bảng chat giúp đóng thanh chat ngay lập tức, trả lại 100% diện tích màn hình cho bài học. Lịch sử chat được tự động lưu lại trong một biểu tượng nhỏ ở góc để học viên có thể mở lại khi cần mà không bị mất dữ liệu.
