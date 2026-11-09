# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: **Nhóm L3A - Nhóm 4**
- Candidate problem nhóm chọn (1 câu): **Gom và trích xuất lịch học, bài tập, deadline bị phân tán từ nhiều kênh (LMS, Email, Discord, Zalo) vào một lịch theo dõi duy nhất kèm mức độ ưu tiên.**
- Quyết định cuối (Go / Not Yet / No-Go): **Go** (Triển khai thử nghiệm pilot phạm vi nhỏ).

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Hoàng Việt | 2A202603487 | Nhóm trưởng, điều phối, phụ trách vẽ Quy trình & viết Problem Statement | HViettt |
| 2 | Đỗ Tuấn Anh | 2A202603465 | Thành viên, phản biện chính, phụ trách Research giải pháp | (GitHub Tuấn Anh) |
| 3 | Nguyễn Hải Anh | 2A202603484 | Thành viên, phụ trách Kiểm chứng (phỏng vấn Mom Test) & AI Canvas | haianh29112 |
| 4 | Nguyễn Thành Danh | 2A202603493 | Thành viên, phụ trách Cây OST, Ma trận can thiệp & Đánh giá 4 rủi ro | (GitHub Thành Danh) |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Thành Danh | Nguyễn Hoàng Việt | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Hải Anh | Đỗ Tuấn Anh | Assumption map, snapshot phỏng vấn Mom Test |
| CP4 — Research | Đỗ Tuấn Anh | Nguyễn Hải Anh | Bảng research giải pháp có sẵn kèm link |
| CP5 — Quy trình trước/sau | Nguyễn Hoàng Việt | Nguyễn Thành Danh | Quy trình Before/After + bảng so sánh |
| CP5 — Problem Statement v0 | Nguyễn Hoàng Việt | Đỗ Tuấn Anh | Bản Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Hải Anh | Nguyễn Hoàng Việt | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Nguyễn Thành Danh | Cả nhóm | Đánh giá 4 rủi ro + Kết luận Go kèm ngưỡng dừng |

## Cá nhân

### NguyenHoangViet-2A202603487

**Phần việc phụ trách:**
- Điều phối buổi thảo luận nhóm ở CP3; tổng hợp các cluster và cây OST.
- Phụ trách chính vẽ sơ đồ quy trình Trước/Sau (Before/After) và soạn thảo bản Problem Statement v0, v1 ở CP5 và CP6.

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Đưa ra và pitch Card #1 (Tổng hợp lịch học & deadline K5), tạo tiền đề hội tụ cho Cluster A của nhóm.
- Xây dựng chi tiết sơ đồ Before (55 phút) và sơ đồ After (8 phút); thiết lập ranh giới kiểm soát (Boundary: bắt buộc có bước con người bấm xác nhận trước khi lưu sự kiện).
- Viết bản Problem Statement v0 và nâng cấp lên v1 có bổ sung điểm can thiệp AI và tiêu chí đánh giá đầu ra (Eval).

**Bằng chứng (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):**
- `report/team/group_report.md`: Mục 2.1 (dòng #1), Mục 4 (Quy trình trước/sau), Mục 5 (Problem Statement v0), Mục 7 (Problem Statement v1).

**Điều mình học được từ phần nhóm:**
- Hiểu sâu sắc tinh thần "Problem first, not AI first". Ban đầu khi mới nhìn bài toán, nhiều bạn nghĩ ngay đến việc xây dựng bot tự động cào dữ liệu hoặc trợ lý AI toàn năng. Sau khi cả nhóm ngồi lại vẽ quy trình và phân tích ma trận độ mơ hồ × độ phức tạp, nhóm nhận ra rằng chỉ cần mức Workflow bán tự động có con người duyệt (Human-in-the-loop) là đã giải quyết được 85% thời gian mà rủi ro gần như bằng 0.

### DoTuanAnh-2A202603465

**Phần việc phụ trách:**
- Người phản biện chính trong buổi pitch CP3; phụ trách tìm kiếm và đối chiếu các giải pháp có sẵn trên thị trường ở CP4.3.

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Đặt câu hỏi phản biện sắc bén cho các card của nhóm (như hỏi về tính sư phạm của AI chấm bài, hỏi về việc có cần AI không nếu đã có Google Calendar).
- Thực hiện research 3 công cụ: Notion Calendar, Canvas Student, Motion AI Calendar; chỉ ra bài học cho nhóm là không nên tạo thêm app lịch mới mà nên tận dụng API lịch có sẵn.

**Bằng chứng:**
- `report/team/group_report.md`: Mục 2.1, Mục 3.3 (Bảng research giải pháp có sẵn).

**Điều mình học được từ phần nhóm:**
- Nghiên cứu giải pháp có sẵn giúp nhóm không phải "phát minh lại chiếc bánh xe" và tránh ảo tưởng về việc tự xây một hệ thống phức tạp khi thị trường đã có các công cụ giải quyết được phần lớn bài toán.

### NguyenHaiAnh-2A202603484

**Phần việc phụ trách:**
- Lập Assumption Map và phụ trách thực hiện phỏng vấn người thật (The Mom Test) ở CP4; xây dựng AI Canvas rút gọn và tiêu chí Eval ở CP6.

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Thực hiện phỏng vấn sâu 2 sinh viên trong lớp theo đúng 3 luật của Mom Test; ghi chép 2 bản Interview Snapshot chi tiết.
- Điền bảng AI Canvas rút gọn (Prediction $\rightarrow$ Judgment $\rightarrow$ Action $\rightarrow$ Outcome) và xây dựng 4 tiêu chí Eval kiểm tra đầu ra của AI.

**Bằng chứng:**
- `report/team/group_report.md`: Mục 3.1, Mục 3.2 (Snapshot #1 & #2), Mục 6.3, Mục 7.2.

**Điều mình học được từ phần nhóm:**
- Học được cách phỏng vấn không mớm cung: hỏi về những hành vi cụ thể và tổn thất đã xảy ra trong quá khứ thay vì hỏi "bạn có thích tính năng này không". Những lời khen xã giao không phải là bằng chứng xác thực.

### NguyenThanhDanh-2A202603493

**Phần việc phụ trách:**
- Xây dựng cây Opportunity Solution Tree (OST) và bảng chấm điểm ở CP3; phụ trách phân tích ma trận can thiệp và đánh giá 4 rủi ro ở CP6.

**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Thiết lập cây OST với đúng 1 Outcome gốc và lọc bỏ các giải pháp đội lốt opportunity; chấm điểm shortlist 3 candidate.
- Phân tích ma trận độ mơ hồ × độ phức tạp; so sánh 4 mức No AI / Rule / Workflow / Agent; đánh giá 4 rủi ro Value, Usability, Feasibility, Viability và xác lập ngưỡng dừng đo lường được.

**Bằng chứng:**
- `report/team/group_report.md`: Mục 2.2, 2.3, 2.4, Mục 6.1, 6.2, Mục 8 (Bốn rủi ro và Quyết định Go).

**Điều mình học được từ phần nhóm:**
- Học được cách ra quyết định Go/No-go có căn cứ dựa trên 4 rủi ro chứ không dựa vào cảm tính; hiểu rõ sự khác biệt giữa Rule, Workflow và Agent để chọn phương án tối giản, hiệu quả nhất.
