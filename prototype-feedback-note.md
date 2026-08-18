# Prototype Feedback Note

**Case:** Case A — AI Tutor: Diagnostic Refresher  
**Người thực hiện thử nghiệm (Facilitator):** Nguyễn Trí Trung — 2A202601594  
**Người tham gia thử nghiệm (Tester):** Đỗ Minh Quân (Học viên lập trình JavaScript cơ bản, 21 tuổi)  
**Option thử nghiệm chính:** Option A — System-Led Diagnostic (AI-Driven)  
**Ngày thử nghiệm:** 18/8/2026  

---

## 1. Mục tiêu thử nghiệm
* Đánh giá xem học viên có sẵn sàng để hệ thống tự chẩn đoán bằng câu hỏi trắc nghiệm hay không.
* Quan sát phản ứng và tốc độ xử lý khi AI đưa ra câu hỏi chẩn đoán ngẫu nhiên.
* Xác định xem học viên có hiểu cách thoát khỏi luồng chẩn đoán và lấy giải thích trực tiếp hay không (Human Control).

---

## 2. Kịch bản & Nhiệm vụ thực tế
Tester được yêu cầu giải quyết nhiệm vụ: Đang viết code in ma trận số bằng vòng lặp For lồng nhau nhưng bị sai chỉ mục `i` và `j`. Tester bấm nút "Tôi vẫn chưa hiểu" để được trợ giúp giải quyết lỗ hổng này.

---

## 3. Ghi chép chi tiết quá trình quan sát (Observations)

### Khâu bấm nút & Kỳ vọng ban đầu:
* **Hành vi:** Tester đọc đề bài, chạy thử thấy sai kết quả. Loay hoay sửa code trong 1 phút nhưng vẫn sai, sau đó bấm nút "Tôi vẫn chưa hiểu".
* **Kỳ vọng:** Tester nghĩ bấm nút sẽ ra ngay câu trả lời giải thích tại sao code của mình sai hoặc cho code đúng.
* **Quote:** *"Em tưởng bấm nút này nó sẽ quét code hiện tại của em và chỉ ra lỗi sai syntax hoặc logic của code ma trận luôn."*

### Khâu chẩn đoán bằng câu hỏi (MCQ Diagnostic):
* **Hành vi:** Khi hệ thống hiển thị thông báo "Trả lời nhanh 2 câu hỏi...", Tester hơi khựng lại. Đọc câu hỏi chẩn đoán thứ nhất (về cách biến chạy trong vòng lặp lồng nhau hoạt động) mất 25 giây để suy nghĩ rồi chọn đáp án. Câu hỏi thứ hai mất 15 giây.
* **Cảm xúc:** Hơi bất ngờ và có chút bực mình vì đang muốn có kết quả nhanh mà lại phải làm bài kiểm tra.
* **Quote:** *"Đang kẹt bài tập lại bắt làm quiz ngắn làm em hơi căng thẳng. Nhưng câu hỏi thiết kế khá hay, trực quan nên em cũng đoán được mục đích của hệ thống."*

### Khâu tiếp thu Refresher (Bài ôn tập ngắn):
* **Hành vi:** Hệ thống chấm điểm quiz và chọn khái niệm "Sự độc lập của biến chỉ mục vòng lặp con" để giải thích. Tester đọc lướt qua đoạn giải thích, dừng lại lâu ở phần ví dụ có hình vẽ minh họa luồng chạy của `i` và `j` (dành ra 40 giây để đọc).
* **Kết quả:** Tester hiểu ra là mình đã nhầm biến `j` thành `i` ở vòng lặp trong.
* **Quote:** *"À, phần giải thích trực quan bằng sơ đồ luồng này rất dễ hiểu. Nhờ cái này em mới thấy mình gõ nhầm i với j ở trong code."*

### Khâu kiểm soát & Thoát hiểm (Human Control):
* **Hành vi:** Khi được hỏi về khả năng tự kiểm soát, Tester chỉ ra nút "Xem giải thích trực tiếp" nhưng thừa nhận lúc đầu không chú ý vì nút này thiết kế nhỏ dưới chân trang. Tester cũng dễ dàng tìm thấy nút "Quay lại bài" ở góc phải để đóng bảng hỗ trợ.
* **Quote:** *"Nếu em đang vội, em sẽ muốn bỏ qua quiz này ngay. Nút bỏ qua nên làm nổi bật hơn một chút để em đỡ có cảm giác bị ép buộc."*

---

## 4. Tóm tắt kết quả
* **Tỷ lệ hoàn thành nhiệm vụ (Task Completion Rate):** 100% (Tester trả lời xong quiz chẩn đoán, đọc hiểu giải thích và tìm ra lỗi sai để sửa code).
* **Thời gian thực hiện (Time on Task):** 2 phút 15 giây.
* **Pain point chính:** 
  * Cảm giác bị "ép buộc" làm quiz khi đang bị kẹt bài tập.
  * Kỳ vọng ban đầu bị lệch (muốn sửa code trực tiếp thay vì chẩn đoán kiến thức nền).
* **Điểm sáng:** Đoạn giải thích bằng sơ đồ trực quan cực kỳ hiệu quả, giúp tester tự ngộ ra lỗi sai mà không cần chỉ thẳng lỗi trong code bài tập.
