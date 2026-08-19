# Group Feedback Synthesis

## Tổng hợp các phiên feedback

| Người facilitate                  | Người test        | Prototype/Option test                     | Feedback chính                                                                                                                                                                                                                                                  |
| ----------------------------------- | ------------------- | ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Đỗ Thu Liễu - Nguyễn Trí Trung | Phạm Tiến Đại   | Option A – Hỏi trực tiếp giảng viên | Người test thấy chức năng hỏi trực tiếp khá dễ sử dụng và phù hợp khi đang học. Tuy nhiên, cần làm nổi bật trạng thái “Chưa trả lời” để người học biết câu hỏi đã được giảng viên tiếp nhận hay chưa.             |
| Phạm Tiến Đại                   | Tạ Thị Thu Huyền | Option B – Sơ đồ kiến thức          | Người test đánh giá cao khả năng nhìn tổng quan bài học và xem nhanh nội dung từng slide. Tuy nhiên, sơ đồ cần đơn giản, tránh quá nhiều thông tin khiến người học khó theo dõi.                                                 |
| Tạ Thị Thu Huyền                 | Đỗ Thu Liễu      | Option C – Khái niệm nền              | Người test thấy việc bấm vào từ khóa để xem giải thích AI hữu ích, đặc biệt khi không biết kiến thức nền liên quan. Tuy nhiên, cần thiết kế phần thông tin AI ngắn gọn để không che quá nhiều nội dung slide.               |
| Tạ Thị Thu Huyền                 | Phạm Tiến Đại   | Option C – Khái niệm nền              | Người test thích chức năng “Vẫn chưa hiểu” và bài kiểm tra nhanh vì giúp xác định mình đang thiếu kiến thức nào. Tuy nhiên, cần đảm bảo câu hỏi kiểm tra ngắn và kết quả dễ hiểu để không làm gián đoạn việc học. |

## Ba điểm tổng hợp chính (Feedback Synthesis)

1. **Người học cần được hỗ trợ nhanh mà không làm gián đoạn bài giảng.** Các chức năng nên cung cấp thông tin ngắn gọn, dễ hiểu và cho phép người học nhanh chóng quay lại nội dung đang học.

2. **Người học cần biết chính xác mình chưa hiểu phần nào.** Việc chỉ cung cấp giải thích là chưa đủ; hệ thống nên giúp người học xác định từ khóa hoặc kiến thức nền đang bị thiếu.

3. **Giao diện cần hạn chế lượng thông tin hiển thị cùng lúc.** Người test đánh giá cao các chức năng hỗ trợ nhưng nếu cửa sổ thông tin, sơ đồ hoặc nội dung AI quá nhiều sẽ khiến học viên mất tập trung khỏi slide chính.

## Next Change

> Thay đổi cụ thể nhóm sẽ thực hiện tiếp theo dựa trên feedback.

* Ưu tiên phát triển Option C vì đây là phương án giải quyết trực tiếp vấn đề xác định và bổ sung kiến thức nền mà học viên đang thiếu.
* Rút gọn nội dung AI hiển thị trên slide , ưu tiên các ý chính như định nghĩa, kiến thức nền liên quan và tài liệu tìm hiểu thêm; cho phép người học mở rộng khi cần.
* Tối ưu chức năng “Vẫn chưa hiểu” bằng các câu hỏi trắc nghiệm ngắn và kết quả trực quan, giúp học viên nhanh chóng biết mình đang thiếu kiến thức nào.
* Giữ giao diện hỗ trợ ở dạng cửa sổ nhỏ/bên cạnh slide để học viên có thể xem thông tin mà không mất ngữ cảnh của bài giảng.

## Still Unproven

> Những giả định (hypothesis) vẫn chưa được kiểm chứng rõ ràng qua các phiên test.

* Chưa chứng minh được AI có thể xác định chính xác kiến thức nền mà học viên đang thiếu dựa trên kết quả trắc nghiệm và nội dung slide.
* Chưa chứng minh được việc sử dụng chức năng hỗ trợ trong thời gian thực thực sự giúp học viên theo kịp bài giảng tốt hơn so với cách học thông thường.
* Chưa kiểm chứng đầy đủ mức độ chính xác và hữu ích của các tài liệu/link mà AI đề xuất cho từng chủ đề.
* Chưa xác định được mức độ thông tin phù hợp mà học viên muốn xem để vừa hỗ trợ hiểu bài vừa không làm mất tập trung trong quá trình nghe giảng.
