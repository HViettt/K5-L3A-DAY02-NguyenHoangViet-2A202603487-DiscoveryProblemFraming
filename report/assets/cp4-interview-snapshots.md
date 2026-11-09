# CP4 — Danh sách Interview Snapshots (The Mom Test)

Bộ phỏng vấn kiểm chứng thực tế được thực hiện ngày 08/11/2026 và 09/11/2026 với 5 học viên thật thuộc khóa học AI thực chiến K5 và các bạn sinh viên làm đồ án môn học (đạt điều kiện **Bonus B2: từ 5 phỏng vấn trở lên, phỏng vấn người thật theo 3 luật The Mom Test: hỏi về hành vi đã xảy ra, không hỏi giả định tương lai, lắng nghe nhiều hơn nói**).

---

### Interview Snapshot #1

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Học viên K5 (nhóm trưởng nhóm 4 người, sinh viên năm 3 ĐHBK) |
| **Bối cảnh & Thời gian** | Phỏng vấn trực tiếp tại sảnh lab học tập K5, chiều 08/11/2026 |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Tối thứ Năm tuần trước, Coach nhắn trong kênh chat chung là dời lịch nộp checkpoint lab từ 23h59 Chủ Nhật lên 18h00 thứ Bảy để kịp chấm. Tin nhắn bị trôi sau một tràng chém gió meme của cả lớp. Đến trưa thứ Bảy nhóm mình mới ngã ngửa ra, cả bọn phải bỏ ăn trưa hộc tốc ngồi gộp code cho kịp nộp."* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Đợt nộp Checkpoint 2 của Day 01 (02/11/2026), nhóm bị nộp muộn 15 phút do xem nhầm mốc giờ thông báo cũ trên LMS (trên LMS ghi 23h59 nhưng Discord Coach dặn nộp trước 22h00 để review trực tiếp). Bị trừ 1 điểm nộp trễ. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Tự mở Google Keep gõ lại danh sách deadline vào đầu tuần; cài chuông báo thức điện thoại trước giờ nộp bài 1 tiếng; thỉnh thoảng tag hỏi trợ giảng trên Discord. |
| **Mất bao lâu, bao lần?** | Mỗi tuần mất khoảng 40–50 phút lội lại các kênh chat để đối soát mốc giờ; tuần nào cũng lo ngay ngáy bị sót lịch dời. |
| **Insight / opportunity rút ra** | Nỗi đau lớn nhất không phải là không biết có deadline, mà là **các thông báo dời lịch/phát sinh đột xuất bị chìm trong luồng chat tự do**. Cần một cơ chế tự bóc tách các mốc giờ phát sinh ngay khi Coach nhắn và đưa vào bảng lịch tập trung. |

---

### Interview Snapshot #2

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Học viên K5 (người vừa đi làm vừa đi học, 24 tuổi) |
| **Bối cảnh & Thời gian** | Phỏng vấn qua Google Meet, tối 08/11/2026 |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Ban ngày mình đi làm ở công ty không mở Discord lớp liên tục được. Tối về mở ra thấy hơn 300 tin nhắn chưa đọc. Ngồi scroll tìm xem có thông báo gì quan trọng của giảng viên hay link Google Drive tài liệu mới không mất đứt 25 phút, nhiều hôm mệt quá bỏ qua luôn thì y như rằng hôm sau vào lớp không biết đang học đến đâu."* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Tối thứ Ba (04/11), giảng viên gửi link repo tài liệu thực hành và dặn clone trước về máy trước 8h sáng hôm sau. Người được hỏi không đọc kịp tin nhắn trong kênh Discord, sáng hôm sau vào lớp mất 20 phút đầu giờ vật lộn tải môi trường trong khi lớp đã bắt đầu giảng. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Dùng tính năng search của Discord gõ keyword: "deadline", "link", "lịch", "bài tập", nhưng vẫn sót vì nhiều khi Coach nhắn: *"Tối mai nộp nhé cả lớp"* (không có từ 'deadline'). |
| **Mất bao lâu, bao lần?** | Diễn ra hàng ngày (4–5 lần/tuần), mỗi lần mất 15–20 phút lọc tin nhắn rác. |
| **Insight / opportunity rút ra** | Công cụ tìm kiếm từ khóa thông thường (Rule-based) bất lực trước ngôn ngữ tự nhiên không theo khuôn mẫu ("tối mai", "cuối tuần", "trước 8h sáng mai"). Cần LLM hiểu ngữ cảnh thời gian tương đối để trích xuất mốc sự kiện. |

---

### Interview Snapshot #3

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Trợ giảng (TA) khóa học AI K5 kiêm quản lý kênh Discord lớp |
| **Bối cảnh & Thời gian** | Phỏng vấn trực tiếp tại bàn hỗ trợ kỹ thuật, sáng 09/11/2026 |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Khổ nhất là mỗi tuần mình phải trả lời đi trả lời lại cùng một câu hỏi: 'Anh ơi bài này nộp ở đâu?', 'Hôm nay học online hay offline anh?'. Mặc dù BTC đã ghim tin nhắn trên kênh #announcements, nhưng học viên vẫn lười kéo lên xem và vào kênh thảo luận hỏi loạn lên."* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Sáng thứ Hai (03/11), có 7 học viên khác nhau nhắn tin riêng (DM) cho TA hỏi cùng câu hỏi về link nộp bài tập và thời gian mở phòng review. TA mất cả buổi sáng chỉ để copy link gửi lại cho từng người. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Ghim tin nhắn (Pin message) trên Discord; gõ lệnh bot `/faq` thủ công; thỉnh thoảng copy lại nội dung thông báo vào kênh chat chung kèm tag `@everyone`. |
| **Mất bao lâu, bao lần?** | Mất khoảng 1–2 tiếng mỗi tuần trả lời câu hỏi lặp lại về lịch và link nộp bài. |
| **Insight / opportunity rút ra** | **Tín hiệu phản bác quan trọng:** TA chỉ ra rằng nếu BTC đã có kênh `#announcements` ghim tin nhắn mà học viên vẫn không xem thì tạo thêm 1 công cụ mới có thể học viên cũng không xem nếu không tích hợp thẳng vào lịch cá nhân (Google Calendar) mà họ đã có thói quen dùng hàng ngày. |

---

### Interview Snapshot #4

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Sinh viên năm cuối làm Đồ án tốt nghiệp theo nhóm 5 người |
| **Bối cảnh & Thời gian** | Phỏng vấn tại thư viện trường, trưa 09/11/2026 |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Thầy hướng dẫn của mình không bao giờ dùng Google Calendar hay Notion. Thầy toàn nhắn Zalo kiểu 'Chiều thứ 6 thầy rảnh từ 2h đến 4h, nhóm qua bộ môn báo cáo nhé'. Nhóm mình có đứa đọc được đứa không, có lần 2 đứa đến muộn bị thầy mắng vì tội thiếu chuyên nghiệp."* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Tuần trước (30/10), thầy nhắn đổi lịch họp từ 14h sang 16h30 ngay trong nhóm Zalo lớp lúc 12h trưa. Trưởng nhóm đang đi đường không check Zalo kịp, dẫn đến cả nhóm đến ngồi đợi ở cửa văn phòng khoa hơn 2 tiếng đồng hồ. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Trưởng nhóm sau khi đọc tin nhắn của thầy phải tự tay mở Google Calendar của nhóm, tạo sự kiện và gán email của 4 bạn còn lại vào. |
| **Mất bao lâu, bao lần?** | Trung bình 2–3 lần/tuần, mỗi lần tạo và đối soát mất khoảng 10–15 phút. |
| **Insight / opportunity rút ra** | Nhu cầu không phải là một "hệ thống quản lý dự án cồng kềnh", mà là **một cầu nối tự động (bridge) biến tin nhắn chat tự do của giảng viên thành sự kiện Google Calendar chuẩn**. |

---

### Interview Snapshot #5

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Học viên K5 (thành viên nhóm làm lab, chỉ theo dõi lịch qua điện thoại) |
| **Bối cảnh & Thời gian** | Phỏng vấn trực tiếp tại khu tự học, chiều 09/11/2026 |
| **Câu nói đáng nhớ nhất (nguyên văn)** | *"Mình chỉ cần đúng 1 thứ: sáng thứ Hai thức dậy nhìn vào màn hình widget Google Calendar trên điện thoại là thấy hết tuần này phải nộp cái gì vào ngày nào, có link nộp bài gắn sẵn ở đó. Chứ bắt mình mở 3 cái app Discord, Zalo, LMS để lục lọi thì kiểu gì cũng có ngày nộp muộn."* |
| **Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra?** | Đợt nộp bài giữa kỳ môn trước, bài nộp yêu cầu nộp trên Google Drive của lớp nhưng học viên lại nộp lên LMS vì không đọc kỹ thông báo cập nhật link nộp trong Discord. Kết quả hệ thống LMS đóng cổng, phải xin xỏ giảng viên nộp bổ sung qua email. |
| **Hiện đang xử lý bằng cách nào (workaround)?** | Nhờ bạn cùng nhóm "nhắc hộ" mỗi khi sắp đến giờ nộp bài. |
| **Mất bao lâu, bao lần?** | Phụ thuộc hoàn toàn vào bạn bè, thỉnh thoảng mời bạn cốc trà sữa để bạn nhắc bài. |
| **Insight / opportunity rút ra** | **Điểm mấu chốt về Usability:** Người dùng cuối không muốn học thêm giao diện mới (No new UI). Đầu ra bắt buộc phải đồng bộ thẳng vào Google Calendar sẵn có để hiển thị widget trên điện thoại. |
