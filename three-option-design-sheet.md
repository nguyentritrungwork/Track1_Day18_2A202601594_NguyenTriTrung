# Three-Option Design Sheet

> Nếu nhóm dùng board chung (Figma/Miro/Notion...), dán link tại đây và chỉ tóm tắt bên dưới:
> **Link board chung của nhóm:** {{link}}

## Hypothesis Problem

- Học viên khó theo kịp bài giảng vì  **không hiểu kiến thức nền nhưng không biết mình thiếu gì** , đồng thời  **không có thời gian tra cứu hoặc hỏi ngay khi bài giảng vẫn tiếp tục** . Vì vậy, họ thường bỏ qua phần chưa hiểu, khiến  **lỗ hổng kiến thức ngày càng tích tụ và khó theo kịp các nội dung phía sau** .

## Option A:

- **Mô tả:** Khi đang học và không hiểu một nội dung trên slide, học viên có thể nhấn nút “Hỏi” bên dưới slide và nhập câu hỏi. Câu hỏi sẽ được gửi đến giảng viên, đồng thời hệ thống xác định slide chứa nội dung liên quan để giảng viên nhanh chóng biết học viên đang thắc mắc ở phần nào. Giảng viên có thể xem và trả lời câu hỏi ngay trong quá trình giảng dạy. Các câu hỏi được phân loại “Đã trả lời” hoặc “Chưa trả lời” để dễ theo dõi.
- **Giải quyết giả định nào:** Nếu học viên có một cách  đặt câu hỏi nhanh và trực tiếp mà không cần ngắt lời giảng viên , giảng viên sẽ biết chính xác học viên đang gặp khó khăn ở đâu và có thể giải đáp kịp thời, giúp hạn chế việc học viên bỏ qua phần chưa hiểu.
- **Điểm khác biệt so với B/C:** Khác với Option B tập trung vào việc tổng quan và điều hướng kiến thức bằng sơ đồ, và Option C tập trung vào việc xác định, giải thích và bổ sung kiến thức nền bằng AI, Option A tập trung vào tương tác trực tiếp giữa học viên và giảng viên để giải quyết thắc mắc ngay trong buổi học.
- **Người phụ trách:** Đỗ Thu Liễu - Nguyễn Trí Trung

## Option B:

- **Mô tả:** Hệ thống cung cấp nút Sơ đồ tư duy để học viên có thể nhanh chóng xem tổng quan bài học. Khi nhấn vào nút này, hệ thống hiển thị  sơ đồ kiến thức của toàn bộ bài , phân chia nội dung theo từng slide. Học viên có thể nhấn vào từng chủ đề để xem  những nội dung chính cần học . Khi chọn một slide cụ thể, hệ thống mở một cửa sổ thông tin bên cạnh slide, cung cấp tóm tắt nội dung slide, các kiến thức nền liên quan và các tài liệu/link để tìm hiểu thêm .
- **Giải quyết giả định nào:** Nếu học viên có thể  nhanh chóng nhìn thấy bức tranh tổng thể của bài học, biết nội dung quan trọng ở từng slide và được gợi ý kiến thức nền liên quan , họ sẽ dễ xác định mình đang thiếu kiến thức gì và có thể bổ sung sau mà  không cần dừng hoặc làm gián đoạn bài giảng .
- **Điểm khác biệt so với A/C:** Option B tập trung vào việc  giúp học viên nhìn thấy bức tranh tổng thể và cấu trúc kiến thức của toàn bộ bài học , từ đó dễ định hướng và tìm lại nội dung cần học. Trong khi Option A tập trung vào việc  gửi câu hỏi trực tiếp cho giảng viên để được giải đáp , thì Option C tập trung vào phát hiện và lấp đầy lỗ hổng kiến thức nền bằng AI thông qua giải thích từ khóa và bài kiểm tra nhanh.
- **Người phụ trách:** Phạm Tiến Đại

## Option C:

- **Mô tả:** 

Hệ thống bổ sung chức năng “Khái niệm nền” ngay bên dưới slide, mặc định ở trạng thái tắt để không làm gián đoạn quá trình học. Khi bật, các từ khóa quan trọng do giảng viên đánh dấu sẽ được tô vàng trên slide. Học viên có thể nhấn vào từng từ khóa để xem thông tin do AI cung cấp, bao gồm  giải thích khái niệm, vai trò/công dụng và mối liên hệ của khái niệm đó với nội dung trong slide .

Với những từ khóa mới mà giảng viên chưa đánh dấu, học viên có thể bôi đen từ khóa để xuất hiện tùy chọn “Giải thích”. Khi chọn, hệ thống hiển thị một cửa sổ nhỏ chứa phần giải thích do AI tạo ra. Trong cửa sổ này có nút  “Tôi vẫn chưa rõ” . Khi học viên nhấn nút này lần đầu, hệ thống ghi nhận ẩn danh rằng học viên đang gặp khó khăn với từ khóa đó và lưu số liệu để giảng viên theo dõi.

Bên cạnh đó, hệ thống có chức năng “Vẫn chưa hiểu?!” ở phía dưới slide. Khi học viên cảm thấy chưa nắm được nội dung, họ có thể mở chức năng này để thực hiện một bài  trắc nghiệm nhanh kiểm tra kiến thức nền . Dựa trên câu trả lời, hệ thống xác định những khái niệm học viên đã nắm được và những phần kiến thức còn yếu hoặc bị thiếu.

Sau khi hoàn thành, học viên có thể chọn “Xem giải thích” để AI tổng hợp và giải thích các kiến thức còn thiếu, đồng thời liên kết chúng với nội dung đang học trên slide. Hệ thống cũng đề xuất các tài liệu và đường link liên quan để học viên có thể tìm hiểu thêm. Khi đã hiểu, học viên chọn “Tiếp tục học” để đóng phần hỗ trợ và quay lại bài giảng.

Đối với giảng viên, dữ liệu về những từ khóa học viên gặp khó khăn được  ghi nhận dưới dạng ẩn danh . Khi mở  “Luồng giảng viên” , giảng viên có thể xem những từ khóa có số lượt học viên chọn “Tôi vẫn chưa rõ” cao. Từ đó, giảng viên có thể duyệt các từ khóa này, đánh dấu chúng là khái niệm quan trọng và bổ sung thông tin vào slide cho những khóa học sau.

- **Giải quyết giả định nào:** Nếu học viên được hỗ trợ  xác định và giải thích nhanh các từ khóa chưa hiểu ngay trong lúc học , đồng thời có công cụ kiểm tra kiến thức nền khi vẫn còn thiếu, thì họ có thể  xác định chính xác lỗ hổng kiến thức và chủ động bổ sung mà không cần làm gián đoạn bài giảng . Dữ liệu ẩn danh từ nhiều học viên cũng giúp giảng viên nhận biết những khái niệm khó và cải thiện nội dung bài giảng trong các khóa học tiếp theo.
- **Điểm khác biệt so với A/B:** Option C tập trung vào xác định và lấp đầy lỗ hổng kiến thức nền của học viên bằng AI ngay trong quá trình học. Trong khi Option A tập trung vào việc  học viên đặt câu hỏi trực tiếp cho giảng viên , và Option B tập trung vào việc  cung cấp cái nhìn tổng quan, sơ đồ hóa nội dung bài học . Option C nổi bật ở khả năng  giải thích từ khóa, kiểm tra kiến thức nền, xác định phần kiến thức còn thiếu và đề xuất tài liệu để học viên bổ sung .
- **Người phụ trách:** Tạ Thị Thu Huyền

## So sánh nhanh

| Tiêu chí                       | Option A                                                                                             | Option B                                                                                                        | Option C                                                                                                                                   |
| -------------------------------- | ---------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Độ khả thi                    | **Cao** – Chức năng hỏi và quản lý câu hỏi tương đối đơn giản, dễ triển khai | **Cao** – Có thể xây dựng dựa trên nội dung slide và AI để tạo sơ đồ/tóm tắt             | **Trung bình** – Có nhiều chức năng AI, kiểm tra kiến thức và thu thập dữ liệu                                          |
| Mức độ giải quyết vấn đề | **Khá cao** – Giúp học viên được giải đáp trực tiếp khi không hiểu              | **Cao** – Giúp học viên nắm tổng quan, xác định nội dung quan trọng và kiến thức liên quan | **Rất cao** – Có thể xác định từ khóa chưa hiểu, tìm kiến thức nền còn thiếu và hỗ trợ bổ sung kiến thức      |
| Rủi ro/giả định chưa chắc  | **Thấp** – Phụ thuộc vào khả năng giảng viên phản hồi kịp thời                    | **Trung bình** – AI có thể tóm tắt hoặc liên kết kiến thức chưa chính xác                   | **Cao** – AI có thể xác định sai lỗ hổng kiến thức; việc tạo câu hỏi và suy luận kết quả cần độ chính xác cao |

## Lựa chọn cuối để làm prototype

- **Option được chọn:** C
- **Lý do chọn:** Nhóm chọn Option C vì nó giải quyết trực tiếp nguyên nhân khiến học viên bị mất gốc: không biết mình đang thiếu kiến thức nào. Hệ thống không chỉ giải thích từ khóa mà còn xác định kiến thức nền còn thiếu và hỗ trợ học viên bổ sung ngay mà không làm gián đoạn bài giảng.
