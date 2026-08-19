# Track1_Day18

## 1. Thông tin cá nhân và nhóm

- **MHV (mã học viên):** 2A202601594
- **Họ tên:** Nguyễn Trí Trung
- **Tên nhóm:** 666
- **Thành viên nhóm (4 người):**
  1. Đỗ Thu Liễu— MHV: 2A202601898
  2. Tạ Thị Thu Huyền— MHV: 2A202601782
  3. Phạm Tiến Đại — MHV: 2A202601610
  4. Nguyễn Trí Trung — MHV: 2A202601594
- **Case nhóm chọn:**
  - AI Tutor: Diagnostic Refresher: Học viên gặp khó khăn khi theo kịp bài giảng vì không hiểu một số từ khóa hoặc kiến thức nền nhưng không biết mình đang thiếu gì, đồng thời không có thời gian tìm hiểu hoặc hỏi giảng viên khi bài giảng vẫn tiếp tục. Điều này khiến các lỗ hổng kiến thức tích tụ và ảnh hưởng đến việc tiếp thu các nội dung tiếp theo.

## 2. Hypothesis Problem

- Vấn đề giả định (hypothesis): Khi giảng viên đang dẫn dắt một khái niệm mới trên slide, học viên gặp khó khăn trong việc theo kịp bài giảng vì hai rào cản xảy ra cùng lúc: (1) họ không hiểu một từ khóa hoặc bức tranh tổng thể đằng sau khái niệm đó, nhưng không biết chính xác đó là lỗ hổng kiến thức nền nào để tự tra cứu ngay; và (2) ngay cả khi nhận ra mình đang bị hụt, họ không có thời gian để dừng lại tìm hiểu — vì bài giảng vẫn tiếp tục trôi và họ không muốn ngắt lời hoặc làm chậm cả lớp — dẫn đến việc họ im lặng bỏ qua, tiếp tục nghe trong tình trạng mất gốc, và khoảng hụt kiến thức đó dồn lại qua các phần sau của bài giảng.
- Đối tượng người dùng: Học viên AI thực chiến và Giảng Viên
- Giả định cần kiểm chứng: Nếu học viên có thể nhanh chóng xác định phần mình chưa hiểu và nhận được hỗ trợ ngay trong lúc học mà không làm gián đoạn bài giảng, thì họ sẽ dễ dàng theo kịp nội dung và hạn chế tích tụ lỗ hổng kiến thức.

## 3. Three Solution Options

Mô tả ngắn gọn 3 phương án giải pháp và link prototype tương ứng (chi tiết đầy đủ xem tại [three-option-design-sheet.md](three-option-design-sheet.md) và [prototype-link.md](prototype-link.md)).

| Option | Mô tả ngắn                                                                                                                            | Link prototype |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| A      | Hỏi trực tiếp giảng viên: Học viên gửi câu hỏi ngay trên slide để giảng viên giải đáp.                                 | [prototype-link](prototype-link)  |
| B      | Sơ đồ kiến thức: Giúp học viên xem tổng quan bài học, nội dung chính và kiến thức liên quan của từng slide.           | [prototype-link](prototype-link)  |
| C      | Khái niệm nền: AI giải thích từ khóa, kiểm tra kiến thức nền và xác định những phần kiến thức học viên còn thiếu. | [prototype-link](prototype-link)  |

## 4. Đóng góp của tôi trong nhóm

- Option/phần tôi phụ trách: Option A (đồng phụ trách với Đỗ Thu Liễu)
- Shared context / content đã đóng góp: Đóng góp ý tưởng và xây dựng cơ chế hỏi trực tiếp giảng viên; hỗ trợ thiết kế luồng tương tác từ slide đến giảng viên, vẽ wireframe/prototype cho Option A, thiết lập kịch bản kiểm thử cho Option A.
- Human–AI decisions: Sử dụng ChatGPT/Claude để brainstorm, diễn đạt, so sánh các phương án và thiết kế các yếu tố Human Control cho Option A (nút thoát hiểm, thông báo trạng thái nhận câu hỏi).
- Facilitation: Đồng facilitate phiên feedback ngày 19/8/2026, trực tiếp chạy thử nghiệm Option A với tester Phạm Tiến Đại.
- Observation / tổng hợp feedback: Ghi nhận phản hồi của tester Phạm Tiến Đại về Option A (dễ sử dụng, cần làm nổi bật trạng thái phản hồi câu hỏi) và phối hợp cùng nhóm tổng hợp feedback cho cả 3 option.

## 5. Prototype Feedback

- Observation từ phiên tôi facilitate (Tester Phạm Tiến Đại - Option A): Người test thấy chức năng hỏi trực tiếp khá dễ sử dụng và phù hợp khi đang học bài. Tuy nhiên, cần làm nổi bật trạng thái "Chưa trả lời" để người học biết câu hỏi đã được giảng viên tiếp nhận hay chưa.
- Ba feedback synthesis (3 điểm tổng hợp chính):
  * Người học cần được hỗ trợ nhanh mà không làm gián đoạn bài giảng.
  * Giao diện và các nút chức năng cần rõ ràng, dễ hiểu.
  * Nội dung hỗ trợ nên ngắn gọn, chỉ hiển thị thông tin cần thiết để tránh làm người học mất tập trung.
- Next Change (thay đổi tiếp theo sẽ làm): Rút gọn nội dung hiển thị, làm rõ các nút chức năng và tối ưu luồng tương tác để người học có thể nhanh chóng quay lại bài giảng.
- Still Unproven (giả định vẫn chưa được kiểm chứng): Chưa chứng minh được việc sử dụng chức năng hỗ trợ trong thời gian thực thực sự giúp học viên theo kịp bài giảng tốt hơn.

(Chi tiết đầy đủ xem tại [prototype-feedback-note.md](prototype-feedback-note.md) và [group-feedback-synthesis.md](group-feedback-synthesis.md))

## 6. AI Support Log

Tóm tắt AI đã hỗ trợ gì, sai/hời hợt ở đâu, và bạn đã tự sửa gì (chi tiết đầy đủ xem [ai-support-log.md](ai-support-log.md)).

* AI hỗ trợ: Brainstorm 3 phương án, viết và chỉnh sửa mô tả Option A/B/C, hỗ trợ so sánh các phương án và tổng hợp feedback.
* Sai / hời hợt: Một số ý tưởng và đánh giá ban đầu còn chung chung, chưa dựa trên dữ liệu test thực tế.
* Tôi đã tự sửa: Tự chọn lọc, điều chỉnh nội dung theo đúng bài toán, prototype và feedback thực tế của nhóm.
