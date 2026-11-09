# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: **Nhóm L3A - Nhóm 4**
- Thành viên: xem [TEAM.md](../../TEAM.md)
  1. Nguyễn Hoàng Việt (Nhóm trưởng — MSSV: 2A202603487)
  2. Đỗ Tuấn Anh (Thành viên — MSSV: 2A202603465)
  3. Nguyễn Hải Anh (Thành viên — MSSV: 2A202603484)
  4. Nguyễn Thành Danh (Thành viên — MSSV: 2A202603493)
- Candidate problem được chọn (1 câu): **Gom và trích xuất lịch học, bài tập, deadline bị phân tán từ nhiều kênh (LMS, Email, Discord, Zalo) vào một lịch theo dõi duy nhất kèm mức độ ưu tiên.**
- Quyết định cuối: **Go** (triển khai pilot phạm vi nhỏ dạng Workflow hỗ trợ trích xuất lịch).

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

Cả 4 thành viên lần lượt trình bày top 3 Problem Cards của mình (tổng cộng 12 candidate), các thành viên còn lại lắng nghe và đặt câu hỏi phản biện thực tế:

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Hoàng Việt | Khi bắt đầu tuần học mới, muốn nắm toàn bộ mốc sự kiện/deadline học tập tại 1 chỗ duy nhất để không bị trễ hạn checkpoint. | Học viên K5, sinh viên | Lội tin nhắn Discord/Zalo tìm thông báo dời lịch (20') | Nếu Ban tổ chức chỉ dùng 1 link Google Calendar chung thì bài này còn cần AI không? (Hải Anh) |
| 2 | Hoàng Việt | Khi luyện đề thi THPT, muốn biết chính xác dạng bài hay làm sai nhất từ đề PDF để tập trung ôn luyện đúng dạng. | Học sinh lớp 12 | Tự phân loại câu sai và tìm bài tương tự (45') | Đề thi PDF công thức toán và hình vẽ rất khó bóc tách, nhóm có đủ khả năng kỹ thuật không? (Tuấn Anh) |
| 3 | Hoàng Việt | Khi đọc phim X-quang phổi, muốn nhanh chóng phân loại loại trừ ca bình thường để tập trung ca bệnh khó. | Bác sĩ chẩn đoán hình ảnh | Đọc và gõ kết luận lặp lại cho ca bình thường (4–5') | Rủi ro y tế bỏ sót tổn thương cực nguy hiểm, nhóm lấy đâu ra bác sĩ thật để phỏng vấn ở CP4? (Thành Danh) |
| 4 | Tuấn Anh | Khi chấm đợt bài luận, muốn có nhận xét tổng quát và lỗi thường gặp để tiết kiệm thời gian chấm bài. | Giảng viên, giáo viên | Đọc bài, đối chiếu rubric và viết nhận xét (8–15'/bài) | Nhận xét của AI có đảm bảo tính sư phạm không, hay giảng viên vẫn phải đọc lại từ đầu? (Hoàng Việt) |
| 5 | Tuấn Anh | Khi khách hỏi cùng 15–20 câu/ngày, muốn trả lời nhanh theo chính sách để giảm thời gian chờ của khách. | Nhân viên CSKH | Tìm đúng FAQ/chính sách và soạn câu trả lời | Đã thử dùng tính năng tin nhắn nhanh (macro/shortcut) có sẵn trên Zalo/Fanpage chưa? (Hải Anh) |
| 6 | Tuấn Anh | Khi chuẩn bị nộp bài, muốn biết rõ định dạng và các mục bắt buộc để nộp đúng hạn không bị thiếu. | Sinh viên | Đọc đối chiếu rubric dài và kiểm tra checklist bài | Sinh viên chỉ cần 1 checklist tĩnh (file Word/Notion), việc gì phải cần giải pháp phức tạp? (Thành Danh) |
| 7 | Hải Anh | Khi dã ngoại/liên hoan xong, muốn gom ảnh bill và tin nhắn chi tiêu để chia tiền công bằng kèm mã VietQR. | Người đại diện thanh toán | Gõ lại món từ ảnh bill và lội chat xem ai ăn gì (30') | Ảnh bill nhàu hoặc mờ chữ in nhiệt thì OCR có đọc được không, hay lại phải gõ tay? (Hoàng Việt) |
| 8 | Hải Anh | Khi vào đầu tuần học, muốn gom lịch học, deadline từ LMS, Zalo, Mail vào thời khóa biểu duy nhất để không lỡ hẹn. | Sinh viên đại học | Mở lần lượt 4 app khác nhau để kiểm tra và đối chiếu (30') | Có lấy tự động được tin nhắn Zalo/LMS không hay người dùng vẫn phải copy-paste vào? (Thành Danh) |
| 9 | Hải Anh | Khi gom đơn đặt cơm trưa/nước uống nhóm, muốn tính đúng tiền từng người và tiền ship sau giảm giá. | Người gom đơn ăn trưa | Tính toán thủ công tiền lẻ và chia voucher (15') | Các app ShopeeFood/GrabFood đã có tính năng "Đặt nhóm", liệu người dùng có cần tool ngoài? (Tuấn Anh) |
| 10 | Thành Danh | Khi mở sửa file Word/Excel từ mấy hôm trước, muốn biết bản nào mới nhất giữa máy tính, Drive và Mail. | Sinh viên làm việc nhóm | Mở 3–4 file dò thủ công xem bản nào có sửa đổi mới nhất (4–5') | Nếu nhóm rèn thói quen làm chung trên 1 link Google Docs/Drive thì pain này có tự biến mất không? (Hoàng Việt) |
| 11 | Thành Danh | Khi đăng ký các gói dịch vụ trial/trả phí, muốn biết ngày tự động gia hạn để kịp hủy không bị trừ tiền oan. | Người dùng cá nhân | Lục tìm email hóa đơn bị trôi và đăng nhập trang Billing (11') | Đặt nhắc nhở trên Google Calendar ngay lúc bấm đăng ký có đủ giải quyết vấn đề chưa? (Hải Anh) |
| 12 | Thành Danh | Khi có 5–6 bài tập dồn cùng tuần, muốn gom deadline và độ nặng các việc để xếp thứ tự ưu tiên làm trước. | Sinh viên học nhiều môn | Lội chat và đọc lướt yêu cầu bài để ước lượng độ nặng (11') | Khó khăn nhất là đọc hiểu đề để biết bài khó hay dễ, AI có ước lượng đúng độ nặng bài tập không? (Tuấn Anh) |

### 2.2. Cluster

Nhóm gom 12 candidate thành 4 nhóm theo pattern chung:

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| **A. Thông tin & deadline học tập phân tán** | #1 (Việt), #6 (Tuấn Anh), #8 (Hải Anh), #12 (Thành Danh) | Thông tin bài tập, deadline, lịch học nằm rải rác trên nhiều kênh (LMS, Mail, Discord, Zalo) khiến sinh viên mất thời gian tổng hợp, dễ bỏ sót hoặc ước lượng sai thứ tự ưu tiên. |
| **B. Tài chính & thanh toán nhóm** | #7 (Hải Anh), #9 (Hải Anh), #11 (Thành Danh) | Chi phí, hóa đơn, đăng ký dịch vụ bị phân mảnh, tốn thời gian tính toán bóc tách và tạo mã thanh toán thủ công. |
| **C. Hỗ trợ học thuật & đánh giá chuyên sâu** | #2 (Việt), #4 (Tuấn Anh) | Đọc hiểu tài liệu dài (bài luận, đề thi PDF) để phân loại kiến thức hoặc chấm điểm nhận xét. |
| **D. Vận hành & quản lý dữ liệu lặp lại** | #3 (Việt), #5 (Tuấn Anh), #10 (Thành Danh) | Xử lý dữ liệu lặp đi lặp lại hàng ngày (phim X-quang, ticket CSKH, phiên bản file). |

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Giảm thời gian sinh viên dành cho việc dò tìm, tổng hợp và sắp xếp lịch học/deadline từ 55 phút/tuần xuống dưới 10 phút/tuần
├── Opportunity 1: Thông báo deadline và lịch học bị phân tán trên 3–4 nền tảng khác nhau (LMS, Discord, Zalo, Outlook)
├── Opportunity 2: Thông báo dời lịch/bài tập thường viết bằng văn bản tự do trong nhóm chat, không có định dạng chuẩn nên dễ bị trôi tin nhắn
└── Opportunity 3: Khó ước lượng độ nặng và thời hạn của từng bài tập để xếp thứ tự ưu tiên làm việc hợp lý
```

**Những ý đã gạch bỏ vì là solution đội lốt opportunity:**
- ✗ *"Xây dựng một trợ lý AI toàn năng tự động đăng nhập mọi tài khoản và làm bài tập thay sinh viên"* (Solution quá viển vông).
- ✗ *"Dashboard tự động cào dữ liệu từ Zalo và Discord"* (Solution kỹ thuật, vướng rào cản API).
- ✗ *"Bot nhắc việc tự động trên Telegram"* (Solution công cụ).

### 2.4. Chấm điểm shortlist (1–5)

Nhóm chọn 3 candidate tiêu biểu từ các cluster để chấm điểm trên 7 tiêu chí:

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **1. Gom và trích xuất lịch học/deadline phân tán** (Cluster A — Việt #1, Hải Anh #8, Danh #12) | 5 | 5 | 5 | 4 | 5 | 5 | 5 | **34** |
| **2. Bóc tách hóa đơn ăn uống & chia tiền VietQR** (Cluster B — Hải Anh #7) | 5 | 4 | 4 | 4 | 4 | 4 | 4 | **29** |
| **3. Chấm bài luận tự động theo rubric** (Cluster C — Tuấn Anh #4) | 4 | 4 | 3 | 4 | 3 | 4 | 3 | **25** |

**Candidate được chọn:** **Gom và trích xuất lịch học, deadline phân tán từ các kênh chat/LMS vào lịch theo dõi tập trung (Candidate 1).**

**Vì sao chọn:**
1. **Sự đồng thuận cao nhất:** Có tới 3/4 thành viên trong nhóm (Việt, Hải Anh, Danh) đều đưa ra bài toán này trong CP2 dưới các góc độ khác nhau.
2. **Cực kỳ khả thi để kiểm chứng (CP4):** Toàn bộ thành viên và các bạn học trong lớp K5 đều là đối tượng thụ hưởng trực tiếp, có thể phỏng vấn người thật ngay lập tức mà không cần tìm người ngoài.
3. **Quy trình và dữ liệu rõ ràng:** Input là văn bản thông báo tự do, output là sự kiện lịch có ngày giờ chuẩn hóa; rất phù hợp để so sánh ranh giới giữa Rule vs Workflow.

**Vì sao loại các candidate còn lại:**
- *Loại Candidate 2 (Chia tiền hóa đơn):* Ý tưởng hay nhưng phụ thuộc nhiều vào chất lượng ảnh chụp bill (nhàu, mờ) và các app ăn uống/ngân hàng đã bắt đầu tích hợp chia tiền.
- *Loại Candidate 3 (Chấm bài luận):* Nhóm không có giảng viên thật để phỏng vấn kiểm chứng chuyên môn trong buổi lab; yêu cầu sư phạm và ngữ cảnh chấm điểm quá phức tạp.

**Xử lý bất đồng:** Ban đầu Hải Anh rất thích bài toán chia tiền VietQR (#7) vì tính ứng dụng cao trong sinh hoạt. Tuy nhiên sau khi Tuấn Anh và Danh chỉ ra rằng bài toán gom lịch học/deadline có tới 3 bạn cùng đau, tiết kiệm thời gian hàng tuần cho cả nhóm và dễ kiểm chứng ở CP4 hơn, Hải Anh đã đồng ý chuyển sang hội tụ bài toán số 1.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

Nhóm liệt kê 5 giả định quan trọng nhất và đánh giá theo 2 trục:

| # | Giả định | Loại | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên khác cũng mất trên 40 phút mỗi tuần và từng trễ hạn do thông báo phân tán | Value | 5 | 2 | **CÓ** (Kiểm chứng ngay) |
| 2 | Người dùng chấp nhận copy-paste văn bản thông báo hoặc forward tin nhắn vào một nơi tập trung thay vì bắt buộc hệ thống phải tự động đăng nhập cào dữ liệu | Usability | 5 | 2 | **CÓ** (Kiểm chứng ngay) |
| 3 | AI có thể trích xuất chính xác 95%+ ngày, giờ, deadline từ các đoạn chat viết tắt, ngôn ngữ tự nhiên | Feasibility | 4 | 3 | Không (đã có benchmark LLM) |
| 4 | Người dùng không muốn giao toàn quyền cho AI tự tạo lịch mà muốn bấm duyệt/xác nhận trước khi thêm vào Google Calendar | Usability | 4 | 2 | **CÓ** |
| 5 | Các trường đại học/khóa học không thể ép toàn bộ giảng viên chỉ dùng đúng 1 kênh thông báo duy nhất | Viability | 4 | 4 | Không (thực tế đã chứng minh) |

**Giả định nhóm kiểm chứng trong buổi này:** Giả định #1 (nỗi đau và tần suất trễ hạn thật) và Giả định #2 (thao tác người dùng sẵn sàng làm).

### 3.2. Kiểm chứng

Nhóm tiến hành phỏng vấn nhanh 2 bạn học viên ở nhóm khác trong lớp học theo 3 nguyên tắc của **The Mom Test** (hỏi hành vi quá khứ, không hỏi ý tưởng tương lai, nói ít nghe nhiều):

#### Interview Snapshot #1

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Bạn N.V.T — Sinh viên năm 3 ngành CNTT, đang học 6 môn trên trường và tham gia khóa học K5 |
| **Câu nói đáng nhớ nhất** | *"Tuần trước thầy báo dời hạn nộp đồ án trên kênh chat Discord lúc 11h đêm, mình không để ý nên tưởng deadline cũ, suýt nữa làm thâu đêm vô ích."* |
| **Lần gần nhất gặp vấn đề** | Tối thứ Năm tuần trước: Tìm lại link Zoom buổi mentoring trên kênh Zalo bị trôi mất 15 phút, phải đi nhắn tin riêng cho bạn cùng nhóm. |
| **Cách xử lý hiện tại (workaround)** | Tự ghi vào sổ tay hoặc dùng app Sticky Notes trên Windows, nhưng hễ có lịch đổi là quên cập nhật vào sổ. |
| **Mất bao lâu, bao lần** | Mất khoảng 10 phút mỗi ngày (tổng khoảng 50–60 phút/tuần); trung bình 1 tháng bị sót 1 thông báo quan trọng. |
| **Insight rút ra** | Người dùng không ngại copy tin nhắn, cái họ ngại là phải nhớ mở sổ ra xem; họ muốn sự kiện tự nhảy vào Google Calendar trên điện thoại. |

#### Interview Snapshot #2

| Trường | Nội dung |
|---|---|
| **Người được hỏi** | Bạn L.T.M — Sinh viên năm 4, đang vừa đi thực tập vừa hoàn thành khóa luận tốt nghiệp |
| **Câu nói đáng nhớ nhất** | *"Thông báo trên LMS thì chuẩn nhưng ít khi cập nhật đột xuất; còn Discord và Zalo thì thông báo liên tục nhưng trôi nhanh như lũ, không tài nào lội hết được."* |
| **Lần gần nhất gặp vấn đề** | Đầu tuần này: Bị phạt nộp bù bài tập vì nộp theo lịch trên slide cũ, không đọc tin nhắn đính chính của trợ giảng ghim trên chat. |
| **Cách xử lý hiện tại (workaround)** | Cứ đầu tuần bỏ ra 30 phút mở hết email, LMS và nhóm chat để tự gõ vào Google Calendar. |
| **Mất bao lâu, bao lần** | Mất khoảng 40–50 phút/tuần; kỳ này đã 2 lần nộp bài sát nút dưới 15 phút vì nhớ nhầm giờ. |
| **Insight rút ra** | Cần hiển thị rõ nguồn tin nhắn trích xuất từ đâu để đối chiếu khi cần kiểm tra lại. |

#### Tổng hợp tín hiệu kiểm chứng:

| Nguồn | Số người / mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sâu The Mom Test | 2 sinh viên | Cả 2 đều mất 40–60 phút/tuần; đều từng bị trễ hạn hoặc suýt trễ hạn do thông báo trôi trên chat; đều dùng Google Calendar làm đích đến cuối cùng. | Nếu một môn học mà giảng viên chỉ dùng duy nhất 1 trang LMS chuẩn chỉ thì sinh viên không bị đau; nỗi đau chỉ bùng nổ khi môn học dùng kênh chat không chính thức (Zalo/Discord). |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
- Ban đầu nhóm định làm cho "tất cả các kênh học tập". Sau phỏng vấn, nhóm **thu hẹp phạm vi**: tập trung giải quyết nút thắt ở các **thông báo văn bản tự do, phi cấu trúc trên các kênh chat (Discord/Zalo/Telegram)** và email, vì đây là nơi phát sinh thông tin dời lịch và dễ trôi nhất.

### 3.3. Research giải pháp đã có

Nhóm khảo sát 3 công cụ/pattern phổ biến hiện nay:

| Công cụ / pattern | Link nguồn | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Notion Calendar** | [notion.com/calendar](https://www.notion.com/product/calendar) | Hiển thị lịch tập trung và đồng bộ Google Calendar | Giao diện đẹp, liên kết mượt mà với database Notion | Người dùng vẫn phải tự gõ tay deadline vào database; không có tính năng đọc hiểu đoạn chat tự do để bóc tách ngày giờ | Công cụ hiển thị đã rất mạnh, nhóm không nên tạo thêm 1 cái app lịch mới mà nên tích hợp xuất dữ liệu vào lịch sẵn có |
| **Canvas Student / LMS App** | [instructure.com/canvas](https://www.instructure.com/canvas) | Tự động đồng bộ bài tập từ web trường về lịch điện thoại | Dữ liệu chính thức, đồng bộ 100% chuẩn xác | Chỉ đọc được bài tập tạo chính thức trên hệ thống; hoàn toàn bất lực trước các thông báo dời lịch, nhắc nhở miệng trên Discord/Zalo | Khoảng trống lớn nhất nằm ở kênh chat phi cấu trúc, không nằm ở hệ thống LMS |
| **Motion AI Calendar** | [usemotion.com](https://www.usemotion.com) | Tự động xếp lịch làm việc dựa trên deadline và độ ưu tiên | Tự tính toán thời gian rảnh và sắp xếp lịch thông minh | Phức tạp, giá rất đắt ($19–34/tháng), đòi hỏi quyền truy cập sâu vào toàn bộ lịch cá nhân, không tối ưu cho tiếng Việt | Đa số sinh viên chỉ cần mức hỗ trợ đơn giản (Workflow trích xuất và đề xuất), không cần AI tự quyết (Agent) vừa tốn kém vừa khó kiểm soát |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại (Before)

```text
HIỆN TẠI — Tổng thời gian: 55 phút/tuần (Thủ công 100%)

[1. Mở LMS check deadline: 10']
         ↓
[2. Lội tin nhắn Discord/Zalo/Email tìm thông báo dời lịch: 20'] ← BOTTLENECK CHÍNH
         ↓
[3. Đọc yêu cầu bài tập để ước lượng độ khó: 10']
         ↓
[4. Tự gõ deadline và sự kiện vào Google Calendar/sổ tay: 10']
         ↓
[5. Nhắn tin hỏi lại bạn cùng nhóm để xác nhận: 5']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | Tài khoản LMS trường | Danh sách hạn nộp chính thức | 10 phút (đầu tuần) | Thường chỉ có hạn chót, không có thông báo đổi lịch đột xuất |
| 2 | Sinh viên | Kênh chat Discord, Zalo, Email | Các tin nhắn văn bản thông báo rời rạc | **20 phút / lần (BOTTLENECK)** | Tin nhắn trôi nhanh, văn bản viết tắt, không có cấu trúc cố định |
| 3 | Sinh viên | Đề bài, yêu cầu bài tập | Ước lượng độ nặng (dễ/vừa/khó) | 10 phút | Sinh viên tự nhẩm tính thời gian cần làm |
| 4 | Sinh viên | Danh sách việc đã lọc | Sự kiện trên Google Calendar / sổ | 10 phút | Gõ thủ công từng dòng tiêu đề, ngày, giờ |
| 5 | Sinh viên | Tin nhắn hỏi bạn bè | Lời xác nhận mốc thời gian | 5 phút | Xác nhận lại xem mình có đọc sót thông báo nào không |

**Bottleneck chính:** Bước 2 — Mất tới 20 phút mỗi tuần chỉ để lội hàng trăm tin nhắn chat và email tìm kiếm xem giảng viên/coach có dời lịch hay thông báo thêm bài tập mới không.

---

### 4.2. Quy trình tương lai (After)

```text
TƯƠNG LAI — Tổng thời gian: 8 phút/tuần (Workflow kết hợp Rule & AI)

[1. Forward / Dán đoạn chat thông báo vào tool: 1'] ← CON NGƯỜI
         ↓
[2. AI đọc hiểu & bóc tách Tên việc, Deadline, Môn học: 5 giây] ← AI (INTERVENTION POINT)
         ↓
[3. Sinh viên xem bản preview, chỉnh sửa nếu cần & bấm DUYỆT: 2'] ← CON NGƯỜI (BOUNDARY & CONTROL)
         ↓
[4. Tự động đồng bộ sự kiện vào Google Calendar qua API: 2 giây] ← RULE / SCRIPT
         ↓
[5. Định kỳ hiển thị checklist 3 việc ưu tiên trong tuần: 5'] ← RULE (Không cần AI)

* Phương án quay về (Fallback): Nếu AI trích xuất sai ngày giờ -> Sinh viên sửa trực tiếp trên ô form trong 10 giây; nếu tool lỗi -> mở link gốc đính kèm xem tin nhắn gốc.
```

---

### 4.3. Before / After

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| **Số bước** | 5 bước thủ công | 4 bước bán tự động | Giảm các bước dò tìm lặp lại |
| **Tổng thời gian** | ~55 phút/tuần | ~8 phút/tuần | **Giảm ~85% thời gian** |
| **Số bước thủ công** | 5 bước | 2 bước (dán tin nhắn + duyệt) | Con người chỉ đóng vai trò kiểm duyệt |
| **Bottleneck chính** | Lội tìm tin nhắn chat | Duyệt bản nháp trích xuất | Chuyển từ "tìm kiếm" sang "xác nhận" |
| **Rủi ro mới phát sinh** | Bỏ sót do không đọc tin | AI trích xuất nhầm thứ/ngày do format lạ | Giải quyết bằng bước Preview có người duyệt 100% |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đại học / học viên khóa công nghệ học nhiều môn cùng lúc, tiếp nhận thông báo qua cả LMS và các nhóm chat (Discord, Zalo, Email). |
| **Quy trình** | Hàng tuần: Kiểm tra LMS $\rightarrow$ Lội tin nhắn chat tìm thông báo dời lịch $\rightarrow$ Đọc ước lượng độ nặng $\rightarrow$ Tự gõ lịch vào Calendar $\rightarrow$ Hỏi lại bạn bè xác nhận. |
| **Bottleneck** | Khâu lội tìm và bóc tách các mốc thời gian từ tin nhắn văn bản tự do trên Discord/Zalo (mất 20 phút/tuần, thông tin dễ bị trôi). |
| **Impact** | Tốn 55 phút/tuần cho việc gom lịch; trung bình 1–2 lần/học kỳ bị trễ hạn nộp bài hoặc vào muộn buổi học do nắm thông tin sai lệch. |
| **Success Metric** | • **Baseline:** Mất 55 phút/tuần; tỷ lệ trễ hạn 1–2 lần/kỳ.<br>• **Target:** Giảm thời gian tổng hợp xuống dưới 10 phút/tuần; số lần trễ hạn/quên lịch giảm về 0.<br>• **Cách đo:** Bấm giờ tự ghi chép thời gian gom lịch và đếm số sự kiện bị bỏ sót trong 3 tuần thử nghiệm. |
| **Boundary** | AI **tuyệt đối không được tự ý** ghi trực tiếp sự kiện vào lịch cá nhân của sinh viên mà không có nút bấm xác nhận (Human-in-the-loop); AI không được tự trả lời tin nhắn trên nhóm chat. |

**Phản biện nhận được cho v0:**
- *Ý kiến phản biện:* "Nếu AI đọc nhầm deadline thứ Hai thành thứ Ba thì sinh viên vẫn bị trễ bài, lúc đó lỗi thuộc về ai?"
- *Nhóm tiếp thu:* Hoàn toàn đồng ý. Do đó trong thiết kế tương lai, giao diện preview bắt buộc phải bôi đậm dòng chữ gốc trích dẫn và ngày giờ đã đổi ra lịch dương để người dùng liếc mắt kiểm tra trong 2 giây trước khi bấm nút "Thêm vào Calendar".

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ mơ hồ CAO $\times$ Độ phức tạp THẤP-TRUNG BÌNH**.

*Vì sao:*
- **Độ mơ hồ cao:** Tin nhắn thông báo của giảng viên/coach viết bằng ngôn ngữ tự nhiên không theo khuôn mẫu cố định (ví dụ: *"Tối mai nộp nhé"*, *"Dời sang 23h Chủ Nhật tuần sau"*, *"Hạn chót thứ 6 tuần này"*). Các câu này chứa ngữ cảnh tương đối phụ thuộc vào thời điểm gửi tin nhắn, Rule cứng (RegEx) không thể xử lý nổi.
- **Độ phức tạp thấp-trung bình:** Đầu ra chỉ gồm 4 trường dữ liệu rõ ràng (Tên môn/việc, Ngày giờ hạn chót, Link tài liệu, Ghi chú) và chỉ cần 1 bước chuyển tiếp vào Google Calendar qua API chuẩn. Không cần hệ thống đa tác nhân hay suy luận nhiều tầng.

---

### 6.2. So sánh 4 mức can thiệp

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Quy định nhà trường/Ban tổ chức chỉ dùng 1 link Google Calendar hoặc 1 kênh LMS duy nhất | Đủ khi tất cả giảng viên đều tuân thủ kỷ luật 100% | Khó khả thi trong thực tế vì thói quen trao đổi qua chat đã quá phổ biến | Không chọn |
| **Rule** (Code script / RegEx) | Viết biểu thức chính quy (RegEx) lọc từ khóa như "deadline", "hạn nộp", ngày tháng dạng `DD/MM/YYYY` | Đủ khi thông báo viết đúng định dạng chuẩn ngày giờ | Bị gãy ngay khi gặp tiếng Việt tự nhiên: "tối mai", "thứ 7 tuần sau", "sau buổi học 2 ngày" | Không chọn |
| **Workflow** | Người dùng forward tin nhắn $\rightarrow$ **AI trích xuất ngày giờ và ngữ cảnh** $\rightarrow$ Người dùng xem preview duyệt $\rightarrow$ **Rule gọi API Google Calendar** | Đủ cho bài toán này vì giải quyết được ngôn ngữ tự do nhưng vẫn giữ con người kiểm soát | AI có thể hiểu nhầm ngữ cảnh thời gian nếu không truyền kèm timestamp tin nhắn | **CHỌN** |
| **Agent** | AI tự động đăng nhập mọi tài khoản LMS, Discord, Zalo, tự đọc mọi kênh và tự lên lịch làm bài | Đủ khi người dùng muốn ủy thác toàn bộ việc quản lý | Chi phí cao, nguy cơ lộ mật khẩu tài khoản, AI hallucination tự tạo lịch sai mà không ai biết | Không chọn |

**Mức chọn:** **Workflow** (kết hợp AI trích xuất thông tin + Rule đồng bộ lịch qua API + Con người bấm duyệt).

**Vì sao không chọn mức đơn giản hơn (Rule):** Vì thông báo trong các nhóm chat tiếng Việt dùng rất nhiều từ chỉ thời gian tương đối (*"mai"*, *"ngày kia"*, *"cuối tuần này"*, *"sau giờ review"*). Rule cứng bằng từ khóa hoặc RegEx chỉ đạt độ chính xác dưới 40% trên mẫu chat thực tế. Cần LLM để hiểu ngữ cảnh dựa trên mốc thời gian tin nhắn được gửi.

**Vì sao không chọn mức phức tạp hơn (Agent):** Cấp quyền cho một Agent tự do đọc toàn bộ hộp thư và tin nhắn riêng tư là rủi ro bảo mật quá lớn, đồng thời chi phí vận hành token liên tục 24/7 là lãng phí không cần thiết cho một nhu cầu cá nhân.

---

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** | AI dự đoán và trích xuất cấu trúc từ đoạn chat: (1) Tên môn/task, (2) Thời điểm bắt đầu/kết thúc (ISO 8601), (3) Mức độ quan trọng (Gấp / Bình thường), (4) Link nộp bài nếu có. |
| **Judgment** | Người dùng nhìn bản preview đối chiếu với câu trích dẫn gốc: Ngày giờ này có đúng không? Có cần chỉnh sửa tiêu đề không? |
| **Action** | Người dùng bấm nút "Duyệt & Thêm vào Calendar" $\rightarrow$ Hệ thống tự động ghi sự kiện vào Google Calendar của tài khoản. |
| **Outcome** | Sự kiện hiển thị chính xác trên ứng dụng Lịch điện thoại; thời gian hoàn tất thao tác dưới 15 giây. |
| **Input** | (1) Nội dung văn bản tin nhắn được dán vào; (2) Thời điểm tin nhắn được gửi (Timestamp làm mốc tham chiếu ngày hiện tại). |
| **Feedback** | Thống kê số lần người dùng phải chỉnh sửa tay ngày giờ trên ô preview; ghi nhận các mẫu câu AI trích xuất sai để cập nhật few-shot prompt. |

---

### 6.4. Hai câu hỏi của Google PAIR

1. **Người dùng muốn được hỗ trợ (augment) hay giao hẳn việc (automate)?**
   - **Trả lời: Được hỗ trợ (Augment).**
   - *Bằng chứng từ kiểm chứng:* Cả 2 sinh viên được phỏng vấn đều khẳng định không muốn một hệ thống tự động ghi lịch lung tung vào điện thoại của họ. Họ muốn AI làm phần việc mệt mỏi nhất là "đọc hiểu và điền sẵn form", còn họ chỉ cần nhìn lướt qua bấm "OK" là yên tâm nhất.

2. **AI sai kiểu nào tệ hơn: Báo nhầm hay Bỏ sót?**
   - **Trả lời: Bỏ sót tệ hơn nhiều.**
   - *Lý do:* Nếu AI "báo nhầm" (nhận nhầm một tin nhắn thảo luận thành deadline), sinh viên chỉ việc bấm "Hủy" trên bản preview trong 1 giây mà không chịu thiệt hại gì. Nhưng nếu AI "bỏ sót" một hạn nộp bài thật, sinh viên sẽ không biết và bị trượt môn / trừ điểm.
   - *Thiết kế xử lý:* Prompt được tinh chỉnh theo hướng nhạy (high recall): nếu có nghi vấn về mốc thời gian thì cứ trích xuất và gắn nhãn cảnh báo *"Cần kiểm tra kỹ"* để người dùng xác nhận.

---

## 7. Problem Statement v1 + Tiêu chí đánh giá (CP6)

### 7.1. Problem Statement v1

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên đại học / học viên khóa công nghệ học nhiều môn, tiếp nhận thông báo qua cả LMS và các nhóm chat phi chính thức (Discord, Zalo, Email). |
| **Quy trình** | Sinh viên dán đoạn chat thông báo $\rightarrow$ **AI trích xuất ngày giờ & tên việc** $\rightarrow$ Sinh viên xem bản preview và bấm xác nhận $\rightarrow$ **Rule ghi vào Google Calendar qua API**. |
| **Bottleneck** | Khâu đọc hiểu và chuyển đổi các mốc thời gian viết bằng ngôn ngữ tự nhiên thành sự kiện chuẩn xác trên lịch. |
| **Impact** | Giảm thời gian tổng hợp lịch từ 55 phút/tuần xuống dưới 10 phút/tuần; triệt tiêu hoàn toàn rủi ro bị trễ hạn bài tập do trôi tin nhắn. |
| **Success Metric** | • Tỷ lệ trích xuất đúng ngày/giờ: **$\ge$ 95%**.<br>• Thời gian thao tác: **< 15 giây / thông báo**.<br>• Số deadline bị bỏ sót trong kỳ: **0**. |
| **Boundary** | • AI **không được tự động ghi vào lịch** nếu không có xác nhận của người dùng.<br>• AI không tự truy cập vào hòm thư hoặc kênh chat riêng tư nếu không được chủ động cung cấp dữ liệu đầu vào. |
| **AI intervention point** | Bước phân tích ngữ nghĩa tin nhắn (NLP/LLM Entity Extraction) để bóc tách: Tiêu đề việc, Thời gian mốc, Deadline, Link nộp. |
| **Mức chọn** | **Workflow** (Human-in-the-loop). |
| **Rủi ro & người kiểm tra** | • *Rủi ro:* AI hiểu sai ngữ cảnh các từ tương đối ("mai", "tuần sau") nếu thiếu mốc thời gian gửi tin nhắn.<br>• *Người kiểm tra:* Người dùng trực tiếp đối chiếu câu trích dẫn gốc trên giao diện preview trước khi lưu. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| **Quy trình** | Mô tả quy trình thủ công chung chung | Xác định rõ luồng Workflow: Dán tin $\rightarrow$ AI bóc tách $\rightarrow$ Duyệt $\rightarrow$ Sync Calendar | Cần chỉ rõ chính xác AI tham gia ở khâu nào và con người kiểm soát ở đâu |
| **Success Metric** | Giảm thời gian từ 55' xuống < 10' | Bổ sung thêm chỉ số kỹ thuật: độ chính xác trích xuất $\ge$ 95% và thời gian xử lý < 15 giây | Để làm tiêu chí nghiệm thu rõ ràng cho mô hình AI |
| **AI Intervention Point** | Chưa có | Nằm ở khâu bóc tách thực thể ngôn ngữ tự nhiên | Yêu cầu chuẩn hóa của CP6 |

---

### 7.2. Tiêu chí đánh giá đầu ra của AI (Eval Criteria)

Nhóm thiết lập 4 tiêu chí để chấm đầu ra của AI là **Đạt** hay **Không đạt**:

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Đúng mốc thời gian** | Ngày và giờ trích xuất khớp chính xác 100% với ngữ cảnh tin nhắn (quy đổi đúng "Chủ Nhật tuần này" thành ngày dương lịch cụ thể). | Lệch ngày, sai giờ, hoặc lấy nhầm thời gian gửi tin nhắn làm deadline. |
| 2 | **Đúng tên đầu việc** | Tên môn học và nội dung việc ngắn gọn, rõ nghĩa (ví dụ: *"Nộp Lab Day 02 - K5"*). | Tiêu đề quá dài (copy cả đoạn chat) hoặc chung chung vô nghĩa (*"Bài tập"*). |
| 3 | **Không bịa đặt (No Hallucination)** | Mọi thông tin (link, ghi chú, phòng học) phải có nguồn gốc từ đoạn text đầu vào. | Tự suy diễn deadline khi trong văn bản không hề nhắc đến mốc thời gian nào. |
| 4 | **Bảo toàn link nộp bài** | Trích xuất chính xác URL nộp bài hoặc file đính kèm (nếu có trong tin nhắn). | Làm gãy link hoặc bỏ sót link nộp bài. |

---

## 8. Quyết định (CP6)

### 8.1. Đánh giá 4 rủi ro

| Rủi ro | Câu hỏi cốt lõi | Mức độ rủi ro | Lý do & Bằng chứng thực tế |
|---|---|:---:|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **Thấp** (An toàn) | Cả 4 thành viên và 2 người được phỏng vấn đều khẳng định gặp vấn đề này hàng tuần, mất 40–60 phút và từng bị phạt do trễ hạn. Nỗi đau là có thật 100%. |
| **Usability** | Người dùng có dùng được, hiểu và sửa được đầu ra không? | **Thấp** (An toàn) | Giao diện preview dạng form cực kỳ đơn giản (gồm 3 ô: Tiêu đề, Ngày, Giờ kèm nút Add Calendar); người dùng chỉnh sửa được ngay trong 5 giây nếu AI sai. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Thấp** (An toàn) | Bài toán Entity Extraction từ text ngắn là thế mạnh vượt trội của các mô hình LLM hiện nay (Gemini Flash, GPT-4o-mini); API Google Calendar rất sẵn có và miễn phí. |
| **Viability** | Có hợp chi phí, pháp lý, quy định không? Ai vận hành? | **Thấp** (An toàn) | Chi phí gọi API LLM cho 1 đoạn tin nhắn chỉ tốn khoảng $0.0001 (vài đồng VNĐ/lần); không lưu trữ dữ liệu cá nhân nên không vướng bảo mật; người dùng tự dùng token cá nhân hoặc bản free. |

---

### 8.2. Kết luận cuối cùng

**Quyết định:** **GO (Triển khai thử nghiệm phạm vi nhỏ)**.

**Lý do:**
1. Cả 4 rủi ro đều ở mức **Thấp (An toàn)**.
2. Bài toán có giá trị thực tế cao, quy trình rõ ràng và người dùng mục tiêu nằm ngay trong tầm tay để đo lường.
3. Không lạm dụng AI: Giải pháp chọn mức **Workflow bán tự động** (Human-in-the-loop), không chạy theo Agent phức tạp, chi phí gần như bằng 0.

**Pilot nhỏ nhất (MVP):**
- Xây dựng một con Bot Telegram / Webhook Discord đơn giản hoặc 1 trang web 1 trang (Single Page Web):
  - Người dùng dán đoạn tin nhắn thông báo vào ô input.
  - LLM trích xuất cấu trúc và hiển thị bảng preview: `[Tiêu đề] - [Hạn nộp: DD/MM/YYYY HH:mm]`.
  - Có sẵn 1 nút bấm: **"Thêm nhanh vào Google Calendar"** (sinh link URL `calendar.google.com/calendar/render?action=TEMPLATE...`).
- Thử nghiệm trên chính 4 thành viên trong nhóm và 5 bạn cùng lớp trong 2 tuần tiếp theo của khóa học K5.

**Ngưỡng dừng (Stop condition):**
> *"Nếu sau 2 tuần thử nghiệm thực tế với ít nhất 20 thông báo bài tập, mà tỷ lệ người dùng phải gõ lại ngày giờ thủ công vượt quá 30% (AI trích xuất sai trên 30%), hoặc người dùng cảm thấy việc copy-paste tin nhắn vào tool tốn thời gian hơn là tự mở lịch gõ tay, nhóm sẽ **DỪNG dự án** và quay về giải pháp **No AI**: đề xuất Ban tổ chức lớp duy trì nghiêm ngặt 1 file Google Sheet/Calendar chung duy nhất."*

---

## 9. Hạn chế và hướng tiếp theo

- **Hạn chế:** 
  - Tool hiện tại chưa tự động hóa khâu lấy dữ liệu từ các nhóm chat đóng (Zalo) do chính sách bảo mật và không có API công khai của nền tảng này; người dùng vẫn phải chủ động copy hoặc chuyển tiếp tin nhắn.
  - Cần đường truyền mạng để gọi API LLM.
- **Hướng tiếp theo:** 
  - Nghiên cứu tích hợp Extension trên trình duyệt để khi sinh viên đang lướt web LMS hoặc Discord web, chỉ cần bôi đen đoạn text thông báo và click chuột phải chọn *"Thêm vào Google Calendar"*.

---

## 10. Tài liệu tham khảo

1. **Double Diamond Design Model** — British Design Council (2005).
2. **The Mom Test: How to talk to customers & learn if your business is a good idea when everyone is lying to you** — Rob Fitzpatrick (2013).
3. **Continuous Discovery Habits: Discover Products that Create Customer Value and Business Value** — Teresa Torres (2021).
4. **People + AI Guidebook (Google PAIR)** — Google (2019), URL: [pair.withgoogle.com](https://pair.withgoogle.com).
5. **Building Effective Agents** — Anthropic (2024), URL: [anthropic.com/research/building-effective-agents](https://www.anthropic.com/research/building-effective-agents).
6. **Inspired: How to Create Tech Products Customers Love** — Marty Cagan, Silicon Valley Product Group (2017).
7. **Prediction Machines: The Simple Economics of Artificial Intelligence** — Ajay Agrawal, Joshua Gans, Avi Goldfarb (2018).
