# AI Support Log

**Case:** Case A — AI Tutor: Diagnostic Refresher  
**Nhóm:** Nhóm 3  
**Học viên:** Nguyễn Trí Trung — 2A202601594  

Tài liệu này ghi chép lại quá trình tương tác giữa học viên và AI trong việc hoàn thành bài tập Day 18.

---

## 1. AI đã hỗ trợ những gì (What AI Assisted)
* **Khởi tạo cấu trúc:** AI hỗ trợ lập kế hoạch thực hiện (Implementation Plan) và đề xuất các file cần tạo theo đúng yêu cầu cấu trúc thư mục tối thiểu của Day 18.
* **Xây dựng khung giải pháp:** AI giúp chi tiết hóa 3 Option (A, B, C) từ ý tưởng ban đầu của nhóm, làm nổi bật sự khác biệt về mặt cơ chế (Mechanism) và phân chia nhiệm vụ Human-AI.
* **Soạn thảo Feedback & Synthesis:** AI hỗ trợ mô phỏng và cấu trúc hóa các ghi chép kiểm thử (Feedback Note) và tổng hợp phản hồi (Synthesis) dựa trên dữ liệu phỏng vấn thực tế từ Day 17.

---

## 2. Điểm hạn chế / Hời hợt của AI (AI Flaws & Shallowness)
* **Lỗi thiết kế Option (Vi phạm Gate 2):** Trong bản nháp đầu tiên, AI đề xuất 3 option rất giống nhau, chỉ khác biệt về cách bố trí giao diện (layout) và màu sắc của nút bấm. AI chưa tự động nhận diện được rằng điều này sẽ làm nhóm bị đánh giá là "Chưa đạt" ở Gate 2 (Meaningful Options).
* **Mơ hồ về Human Control (Vi phạm Gate 3):** AI đưa ra các cơ chế kiểm soát của con người rất chung chung (ví dụ: "Người dùng có thể bấm nút quay lại") mà không bám sát 4 yếu tố bắt buộc: Expectation, Agency, Evidence/Uncertainty, và Recovery.
* **Kịch bản kiểm thử chưa rõ ràng (Vi phạm Gate 4):** AI đề xuất kịch bản kiểm thử quá rộng ("Học viên làm bài tập JavaScript") khiến tester ngoài nhóm khó có thể tự thực hành nếu không có người hướng dẫn giải thích thêm.

---

## 3. Cách học viên tự rà soát và sửa lỗi (Human Self-Correction)
* **Sửa Gate 2 (Meaningful Options):** Học viên yêu cầu AI thay đổi hoàn toàn cơ chế của 3 option để đảm bảo tính độc lập:
  * Option A phải là **Hệ thống dẫn dắt hoàn toàn** (System-Led với quiz chẩn đoán).
  * Option B là **Hợp tác** (Cooperative với menu lựa chọn chủ động).
  * Option C là **Học viên dẫn dắt** (Conversational chat sidebar đối thoại tự do).
* **Sửa Gate 3 (Human Control):** Học viên yêu cầu chỉ rõ 4 yếu tố kiểm soát cho từng option. Ví dụ trong Option A, bổ sung nút "Xem giải thích trực tiếp (Bỏ qua chẩn đoán)" để tăng Agency, và hiển thị chỉ số độ tin cậy phần trăm của AI để biểu diễn Uncertainty.
* **Sửa Gate 4 (Test-ready):** Học viên giới hạn bài kiểm thử vào một nhiệm vụ cực kỳ cụ thể: "Kẹt ở phần vòng lặp lồng nhau do nhầm lẫn chỉ mục i và j khi in ma trận" giúp tester ngoài nhóm dễ dàng thực hiện độc lập mà không cần facilitator giải thích.
