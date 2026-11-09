# CP6 — Bộ Test Dataset & Tiêu chí Đánh giá Mẫu (Eval Dataset)

Bộ dữ liệu đánh giá gồm **10 test cases mô phỏng các tình huống thực tế** của tin nhắn thông báo tự do từ Giảng viên, Coach, Trợ giảng (TA) trên các kênh chat Discord/Zalo/LMS trong khóa học AI thực chiến K5.

---

### Tiêu chí chấm điểm (4 Eval Criteria)

1. **[E1 - Temporal & Date/Time Accuracy] Độ chính xác thời gian & mốc ngày giờ:**
   - Trích xuất chính xác ngày, giờ bắt đầu và hạn chót (Deadline) từ ngôn ngữ tự nhiên tiếng Việt (bao gồm các từ ngữ tương đối: "tối mai", "thứ 7 tuần này", "trước 22h CN", "cuối tuần sau").
   - Chuẩn hóa thành định dạng ISO 8601 (`YYYY-MM-DDTHH:mm:ss`) hoặc format chuẩn của Google Calendar API.
   - **Đạt:** Sai lệch thời gian bằng 0 phút so với ngữ cảnh gửi tin.
   - **Không đạt:** Sai ngày, lộn AM/PM, hoặc không tính đúng ngày khi có từ "mai", "ngày kia".

2. **[E2 - Event Title & Scope Extraction] Trích xuất tên sự kiện & phân loại đúng phạm vi:**
   - Đặt tên sự kiện ngắn gọn, rõ ràng (ví dụ: `[K5-Lab] Review Checkpoint 2 - Day 02`).
   - Phân loại đúng loại sự kiện: `Lịch học trực tiếp`, `Lịch nộp bài (Deadline)`, `Office Hours / Q&A`, `Lịch họp nhóm`.
   - **Đạt:** Tên sự kiện thể hiện đúng bản chất và mã môn/nội dung.
   - **Không đạt:** Đặt tên chung chung vô nghĩa như "Thông báo", "Học", "Nhắc nhở".

3. **[E3 - Action Item & Link Extraction] Trích xuất hành động & Link liên kết:**
   - Bóc tách đầy đủ link Google Drive, link LMS, link nộp repo GitHub hoặc link Google Meet/Zoom nếu có trong tin nhắn.
   - Trích xuất ngắn gọn yêu cầu hành động (Action item: cần chuẩn bị slide, commit code, hay cài trước thư viện gì).
   - **Đạt:** Link đầy đủ, không bị đứt gãy ký tự; mô tả hành động dưới 20 từ.
   - **Không đạt:** Bỏ sót link nộp bài hoặc bịa ra link không có trong text.

4. **[E4 - Noise Rejection & Hallucination Defense] Khả năng lọc nhiễu & chống ảo giác:**
   - Phân biệt chính xác giữa **tin nhắn thông báo có sự kiện/deadline thật** và **tin nhắn thảo luận, đùa vui, chém gió, câu hỏi han thông thường**.
   - Nếu tin nhắn không chứa sự kiện hoặc mốc thời gian cụ thể: AI phải trả về `is_event: false`, không được tự bịa ra sự kiện.
   - **Đạt:** Từ chối xử lý tin nhắn rác/chém gió với độ chính xác 100%.
   - **Không đạt:** Tự tưởng tượng ra deadline từ một câu nói đùa của học viên.

---

### Bảng 10 Test Cases Chi Tiết (Input Text -> Expected Structured Output)

*Ngữ cảnh mốc thời gian hệ thống giả định khi nhận tin: **Thứ Hai, ngày 09/11/2026 lúc 10:00:00 AM**.*

| # | Tin nhắn đầu vào (Chat Message Input) | Đầu ra mong đợi từ AI (Expected Structured JSON Output) | Đánh giá Đạt / Không đạt |
|---|---|---|---|
| **1** | **Coach nhắn trên kênh Discord #thong-bao-lop lúc 10:15 ngày 09/11/2026:**<br>`@everyone Cả lớp chú ý: Lịch review Checkpoint 2 tối mai (thứ 3) sẽ dời từ 19h30 sang 20h00 nhé. Các nhóm nhớ chuẩn bị sẵn slide và repo GitHub.` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "REVIEW_SESSION",<br>  "title": "[K5] Review Checkpoint 2 (Dời lịch)",<br>  "start_time": "2026-11-10T20:00:00+07:00",<br>  "end_time": "2026-11-10T22:00:00+07:00",<br>  "deadline": null,<br>  "action_required": "Chuẩn bị slide và repo GitHub",<br>  "link": null,<br>  "confidence": 0.98<br>}<br>``` | **ĐẠT** nếu tính đúng "tối mai" là ngày `10/11/2026` lúc `20:00` và ghi chú rõ đây là lịch dời. **TRƯỢT** nếu để 19:30 hoặc sai ngày. |
| **2** | **TA nhắn trên nhóm Zalo môn học lúc 14:00 ngày 09/11/2026:**<br>`Nhắc các bạn hạn chót nộp bài Lab 2 là 23h59 Chủ Nhật tuần này (15/11). Link nộp bài tập tại: https://lms.k5ai.edu.vn/submit-lab2. Nộp muộn sau giờ này hệ thống sẽ tự động đóng cổng.` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "DEADLINE",<br>  "title": "[K5-Lab] Hạn chót nộp bài Lab 2",<br>  "start_time": "2026-11-15T23:59:00+07:00",<br>  "end_time": "2026-11-15T23:59:00+07:00",<br>  "deadline": "2026-11-15T23:59:00+07:00",<br>  "action_required": "Nộp bài Lab 2 trước khi đóng cổng",<br>  "link": "https://lms.k5ai.edu.vn/submit-lab2",<br>  "confidence": 0.99<br>}<br>``` | **ĐẠT** nếu trích xuất đúng deadline `2026-11-15T23:59:00` và giữ nguyên link URL nộp bài chuẩn xác. |
| **3** | **Giảng viên thông báo đổi phòng học đột xuất:**<br>`Do phòng Lab 302 đang sửa điều hòa, chiều nay 14h cả lớp chuyển sang phòng Lab 405 nhà B học nhé. Ai vào muộn tự liên hệ lớp trưởng.` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "CLASS_SESSION",<br>  "title": "[Đổi phòng] Học chiều nay tại Lab 405 nhà B",<br>  "start_time": "2026-11-09T14:00:00+07:00",<br>  "end_time": "2026-11-09T17:00:00+07:00",<br>  "location": "Phòng Lab 405 nhà B",<br>  "action_required": "Chuyển từ Lab 302 sang Lab 405",<br>  "confidence": 0.95<br>}<br>``` | **ĐẠT** nếu nhận diện được "chiều nay" là `09/11/2026` lúc `14:00` và địa điểm là `Lab 405 nhà B`. |
| **4** | **Coach thông báo Office Hours hỗ trợ đồ án:**<br>`Tối thứ 5 tuần này từ 20h đến 21h30 mình sẽ mở room Google Meet giải đáp thắc mắc về pipeline RAG cho các nhóm. Link meet: https://meet.google.com/xyz-k5ai-abc` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "OFFICE_HOURS",<br>  "title": "[Q&A] Office Hours giải đáp pipeline RAG",<br>  "start_time": "2026-11-12T20:00:00+07:00",<br>  "end_time": "2026-11-12T21:30:00+07:00",<br>  "link": "https://meet.google.com/xyz-k5ai-abc",<br>  "action_required": "Hỏi đáp thắc mắc pipeline RAG",<br>  "confidence": 0.98<br>}<br>``` | **ĐẠT** nếu tính đúng "thứ 5 tuần này" là ngày `12/11/2026`, thời gian từ `20:00` đến `21:30` và link meet đầy đủ. |
| **5** | **Tin nhắn chém gió, thảo luận phi sự kiện:**<br>`Hôm nay bài lab khó dã man các ông ạ, tôi ngồi fix bug từ sáng đến giờ chưa xong, tối nay có ai đi làm cốc trà sữa hạ hỏa không?` | ```json<br>{<br>  "is_event": false,<br>  "reason": "Tin nhắn thảo luận cá nhân, rủ đi chơi, không có sự kiện/deadline học tập"<br>}<br>``` | **ĐẠT** nếu từ chối (`is_event: false`). **TRƯỢT** nếu tự động tạo sự kiện "Đi uống trà sữa hạ hỏa" vào lịch học chung. |
| **6** | **Hủy lịch học / Buổi review:**<br>`@channel Thông báo khẩn: Tối nay Coach có việc đột xuất tại công ty nên buổi Mentor 1-on-1 tối nay bị hủy nhé. Lịch bù sẽ thông báo lại vào cuối tuần.` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "CANCEL_EVENT",<br>  "title": "[HỦY LỊCH] Buổi Mentor 1-on-1 tối nay",<br>  "start_time": "2026-11-09T19:30:00+07:00",<br>  "status": "CANCELLED",<br>  "action_required": "Hủy buổi mentor, chờ lịch bù cuối tuần",<br>  "confidence": 0.96<br>}<br>``` | **ĐẠT** nếu nhận diện được hành vi HỦY (`status: CANCELLED`) để kích hoạt chức năng xóa hoặc gạch ngang sự kiện trên Calendar. |
| **7** | **Thông báo có 2 mốc thời gian phụ thuộc nhau:**<br>`Các nhóm nộp bản nháp slide trước 17h thứ 6 ngày 13/11 để Coach duyệt trước. Buổi thuyết trình chính thức sẽ diễn ra lúc 8h30 sáng thứ 7 (14/11).` | ```json<br>[<br>  {<br>    "title": "[Deadline] Nộp bản nháp slide",<br>    "start_time": "2026-11-13T17:00:00+07:00",<br>    "event_type": "DEADLINE"<br>  },<br>  {<br>    "title": "[Lịch học] Buổi thuyết trình chính thức",<br>    "start_time": "2026-11-14T08:30:00+07:00",<br>    "event_type": "CLASS_SESSION"<br>  }<br>]<br>``` | **ĐẠT** nếu tách được thành 2 sự kiện riêng biệt: 1 mốc deadline nộp slide và 1 mốc lịch học thuyết trình. |
| **8** | **Tin nhắn viết tắt, tiếng lóng học đường:**<br>`dl nộp repo github bt tuần 2 là trc 10h tối mai nha ae, k nộp là ăn 0đ đấy` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "DEADLINE",<br>  "title": "[Deadline] Nộp repo GitHub bài tập tuần 2",<br>  "start_time": "2026-11-10T22:00:00+07:00",<br>  "deadline": "2026-11-10T22:00:00+07:00",<br>  "action_required": "Nộp repo GitHub bài tập tuần 2",<br>  "confidence": 0.94<br>}<br>``` | **ĐẠT** nếu dịch đúng từ viết tắt "dl" = Deadline, "bt" = Bài tập, "trc 10h tối mai" = `2026-11-10T22:00:00`. |
| **9** | **Tin nhắn cập nhật yêu cầu (không đổi giờ nhưng đổi link/tài liệu):**<br>`Cập nhật: Link đề bài lab 3 vừa được sửa lại lỗi typo ở câu 4, mọi người tải lại đề mới tại: https://github.com/k5ai/lab3-assignment/releases/tag/v1.1 nhé.` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "UPDATE_RESOURCE",<br>  "title": "[Tài liệu] Cập nhật đề bài Lab 3 (v1.1)",<br>  "link": "https://github.com/k5ai/lab3-assignment/releases/tag/v1.1",<br>  "action_required": "Tải lại đề mới sửa lỗi typo câu 4",<br>  "start_time": null,<br>  "confidence": 0.92<br>}<br>``` | **ĐẠT** nếu phân loại đúng đây là cập nhật tài nguyên/tài liệu, đính kèm link repo mới nhất thay vì tạo lịch sai. |
| **10** | **Tin nhắn mập mờ, thiếu dữ liệu giờ giấc:**<br>`Tuần sau có bài kiểm tra giữa kỳ nhé cả lớp, nhớ ôn tập kỹ các bài từ tuần 1 đến tuần 4.` | ```json<br>{<br>  "is_event": true,<br>  "event_type": "TENTATIVE_NOTICE",<br>  "title": "[Lưu ý] Bài kiểm tra giữa kỳ vào tuần sau",<br>  "start_time": null,<br>  "is_ambiguous": true,<br>  "action_required": "Cần xác nhận lại ngày giờ cụ thể với Giảng viên",<br>  "confidence": 0.65<br>}<br>``` | **ĐẠT** nếu đánh cờ cảnh báo `is_ambiguous: true` và KHÔNG tự đoán mò ngày giờ cụ thể khi tin nhắn chỉ ghi chung chung "tuần sau". |
