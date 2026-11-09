# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: **ihihi**
- Candidate problem nhóm chọn (1 câu): **Khi bước vào giai đoạn luyện đề nước rút (còn 2–3 tháng trước kỳ thi), học sinh lớp 12 muốn biết chính xác dạng bài/chuyên đề vi mô mình hay làm sai nhất dựa trên các đề thi thử PDF đã giải và gom được ngay các câu hỏi tương tự để luyện lại, thay vì mất 45 phút mỗi đề để tự phân loại thủ công hoặc cày đề mới tràn lan mà vẫn lặp lại lỗi cũ.**
- Quyết định cuối (Go / Not Yet / No-Go): **Go** (Phạm vi pilot nhỏ trong 2 tuần với kiến trúc Workflow trên ngân hàng đề PDF có sẵn).

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Nguyễn Hoàng Việt | `2A202603487` | Nhóm trưởng, điều phối thời gian, đề xuất Candidate chính (#2 Phân loại dạng bài sai THPT), viết Problem Statement v0/v1 | `HViettt` |
| 2 | Nguyễn Thành Danh | `2A202603493` | Tech Lead, xây dựng cây OST, research giải pháp có sẵn (Azota, VietJack, NotebookLM), thiết kế quy trình & Eval criteria | `thdanhnguyen` |
| 3 | Đỗ Tuấn Anh | `2A202603465` | Phản biện chính, phụ trách kiểm chứng (Assumption Map, khảo sát 12 người), đối chiếu rubric và rà soát lập luận | *(Tài khoản của Tuấn Anh)* |
| 4 | Nguyễn Hải Anh | `2A202603484` | User Discovery Lead, phụ trách phỏng vấn The Mom Test (4 Snapshots), vẽ sơ đồ Mermaid, thiết kế bộ Eval Dataset | `haianh29112` |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Hoàng Việt, Nguyễn Thành Danh | Đỗ Tuấn Anh, Nguyễn Hải Anh | Bảng 12 pitch, 4 cluster, cây OST, bảng chấm điểm shortlist |
| CP4 — Kiểm chứng | Nguyễn Hải Anh, Đỗ Tuấn Anh | Nguyễn Hoàng Việt, Nguyễn Thành Danh | Assumption Map (5 giả định), 4 Interview Snapshots + khảo sát 12 người |
| CP4 — Research | Nguyễn Thành Danh | Nguyễn Hoàng Việt | Bảng research 4 công cụ có link (Azota, VietJack, Khan Academy, Google NotebookLM) |
| CP5 — Quy trình trước/sau | Nguyễn Thành Danh, Nguyễn Hải Anh | Đỗ Tuấn Anh | Sơ đồ quy trình hiện tại (5 bước, 45' bottleneck) & tương lai (Workflow 6 bước) + bảng before/after |
| CP5 — Problem Statement v0 | Nguyễn Hoàng Việt | Nguyễn Thành Danh | Problem Statement v0 (6 trường) + ghi nhận 3 điểm phản biện |
| CP6 — Mức can thiệp + Problem Statement v1 | Nguyễn Hoàng Việt, Nguyễn Thành Danh | Nguyễn Hải Anh | Ma trận, bảng 4 mức, AI Canvas, câu hỏi PAIR, 5 tiêu chí Eval + 10 test cases, Problem Statement v1 |
| CP6 — Quyết định | Cả nhóm (Hoàng Việt & Thành Danh tổng hợp) | Tuấn Anh, Hải Anh | Bảng đánh giá 4 rủi ro Marty Cagan + Quyết định Go (Pilot 2 tuần) + 2 ngưỡng dừng |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### NguyenHoangViet-2A202603487

**Phần việc phụ trách:**
- Nhóm trưởng điều phối tiến độ, đề xuất bài toán chính **Phân loại dạng bài sai khi luyện thi THPT** (Card #2 trong Top 3 cá nhân).
- Phụ trách chính soạn thảo **Problem Statement v0** và nâng cấp lên **Problem Statement v1** (Mục 5 & 7 trong báo cáo nhóm).
- Đồng thiết kế quy trình Trước/Sau (Before/After) và rà soát đánh giá 4 rủi ro, ngưỡng dừng ra quyết định Go (Mục 8).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Trình bày pitch Card #2, bảo vệ bài toán trước phản biện của nhóm về rủi ro đề PDF không đồng nhất và câu hỏi có hình vẽ.
- Đề xuất giải pháp quy trình: học sinh không cần tự gõ tay lại đề bài, mà sử dụng cơ chế nạp kèm văn bản lời giải chi tiết để AI nhận diện phương pháp giải ẩn sau câu hỏi.
- Trực tiếp soạn thảo bản Problem Statement v0 và nâng cấp lên v1 có bổ sung điểm can thiệp AI, thiết lập Boundary nghiêm ngặt cấm AI tự sáng tác đề mới, và xác định rõ Success Metric định lượng (giảm từ 45' xuống < 10'/đề, độ chính xác $\ge 85\%$).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- `report/team/group_report.md`: Mục 2.1 (dòng #2), Mục 2.4 (lập luận chọn bài toán), Mục 4.1–4.3 (Quy trình trước/sau), Mục 5 (Problem Statement v0), Mục 7 (Problem Statement v1), Mục 8 (Quyết định Go).

**Điều mình học được từ phần nhóm:**
- Hiểu sâu sắc tinh thần "Problem first, not AI first": bài toán ban đầu về tổng hợp lịch học tưởng như rất hay vì nhiều người gặp, nhưng khi phản biện thì nhận ra chỉ cần No AI (Google Calendar chung) là giải quyết được; trong khi bài toán luyện đề THPT mới thực sự có nút thắt cần tới năng lực hiểu ngữ nghĩa của AI.
- Học được cách thiết lập ranh giới (Boundary) và điểm can thiệp (Intervention point) để vừa phát huy thế mạnh của LLM (đọc hiểu văn bản đề + giải), vừa triệt tiêu điểm yếu (không cho phép AI tự chế đề mới gây sai số liệu).

### NguyenThanhDanh-2A202603493

**Phần việc phụ trách:**
- Tham gia pitch 3 Problem Cards cá nhân, đặt câu hỏi phản biện trực tiếp ở CP3 giúp nhóm loại bỏ bài toán chỉ cần No AI (*Tổng hợp lịch học*) và hội tụ về bài toán **Phân loại dạng bài sai khi luyện thi THPT**.
- Phụ trách xây dựng cây OST, phỏng vấn 1 bạn gia sư luyện thi theo The Mom Test và thực hiện phần **Research giải pháp đã có** (Mục 3.3).
- Đồng thiết kế **Quy trình trước/sau** (Mục 4), góp ý nâng cấp **Problem Statement v0 → v1** (xử lý rủi ro đề PDF không đồng nhất, lệch chuyên đề và bài toán có hình vẽ), xây dựng **5 tiêu chí đánh giá (Eval)** và hoàn thiện bộ 10 test cases.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Đặt 2 câu hỏi phản biện trọng tâm ở CP3: (1) Chỉ ra bài *Tổng hợp lịch học* có thể giải quyết bằng 1 link Google Calendar chung (No AI); (2) Chất vấn cách xử lý khi đề thi PDF có cấu trúc không đồng nhất, có hình vẽ không gian/đồ thị và nguy cơ AI phân loại lệch chương trình học — đây trở thành các giả định cốt lõi trong Assumption Map của nhóm.
- Trực tiếp kiểm tra và viết bảng phân tích 4 nền tảng thực tế (Azota, VietJack, Khan Academy, Google NotebookLM) kèm bài học rút ra ở Mục 3.3.
- Đề xuất giải pháp kỹ thuật quan trọng sau kiểm chứng CP4: kết hợp đọc **Văn bản câu hỏi + Văn bản lời giải chi tiết** để vượt qua rào cản hình vẽ, khóa chặt đầu ra vào **Khung Taxonomy 35 dạng bài chuẩn GDPT 2018**, và thiết lập Boundary **cấm AI tự chế đề Toán mới** (chỉ truy xuất từ ngân hàng đề thật).
- Viết 5 tiêu chí Eval ở Mục 7 và xây dựng 10 cặp Input/Expected Output mẫu trong `report/assets/cp6-eval-dataset.md`.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- Báo cáo nhóm: `report/team/group_report.md` (đóng góp chính ở Mục 2.1–2.4, Mục 3.3, Mục 4.1–4.3, Mục 6.2–6.4, Mục 7, Mục 8).
- File phụ lục: `report/assets/cp4-interview-snapshots.md`, `report/assets/cp6-eval-dataset.md`, và ảnh sơ đồ quy trình trong `report/assets/` (`cp5-workflow-future.png`).

**Điều mình học được từ phần nhóm:**
- Học được cách dũng cảm từ bỏ một candidate có nhiều người đề xuất (*Tổng hợp lịch học*) khi phát hiện ra nó chỉ cần 1 link lịch chung, để chọn bài toán có nút thắt thực sự cần tới **Workflow có AI** (*Phân loại dạng bài sai & tìm câu tương tự từ kho đề PDF*).
- Hiểu rõ cách dùng **Rule + Boundary** để kiểm soát điểm yếu của AI: dùng Khung Taxonomy cố định để chống phân loại lệch kiến thức, dùng lời giải chi tiết + cờ cảnh báo `[Có hình vẽ]` để xử lý bài toán hình học/đồ thị, và chỉ truy xuất đề thật thay vì để AI tự chế đề sai số liệu.

### DoTuanAnh-2A202603465

**Phần việc phụ trách:**
- Đóng vai phản biện chính ở CP3, đặt các câu hỏi chất vấn trọng tâm về tính khả thi và rủi ro của từng đề tài.
- Phụ trách xây dựng bảng **Assumption Map** (Mục 3.1) và thực hiện khảo sát định lượng 12 học sinh/gia sư (Mục 3.2).
- Rà soát đối chiếu tiêu chuẩn chấm điểm (Rubric) và lập luận logic trong toàn bộ báo cáo nhóm.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Đặt câu hỏi phản biện trực tiếp ở CP3 giúp nhóm nhận diện sớm rủi ro công thức toán $LaTeX$ và hình vẽ/đồ thị trong đề PDF.
- Lập bảng Assumption Map phân loại 5 giả định theo 4 loại rủi ro (Value, Usability, Feasibility, Viability) và chọn ra các giả định cần kiểm chứng trước.
- Thu thập dữ liệu khảo sát từ 12 học sinh/gia sư: 10/12 người xác nhận gặp tình trạng bỏ qua khâu phân loại câu sai và làm lại bài vì mất quá nhiều thời gian (45 phút/đề).

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- `report/team/group_report.md`: Mục 2.1 (dòng #7, #8, #9), Mục 3.1 (Assumption Map), Mục 3.2 (Bảng tổng hợp khảo sát 12 người), Mục 8.1 (Đánh giá 4 rủi ro).

**Điều mình học được từ phần nhóm:**
- Học được cách kiểm chứng bằng bằng chứng thực tế (evidence-based) thay vì phỏng đoán cảm tính: một giả định dù nghe có vẻ hiển nhiên vẫn phải đo bằng số người gặp thật và hành vi đã xảy ra.
- Hiểu được giá trị của việc phản biện: việc chỉ ra lỗ hổng không phải là bác bỏ ý kiến của bạn, mà là giúp nhóm tìm ra ranh giới kiểm soát an toàn hơn cho sản phẩm.

### NguyenHaiAnh-2A202603484

**Phần việc phụ trách:**
- Phụ trách thực hiện các buổi phỏng vấn sâu theo phương pháp **The Mom Test** ở CP4 (Mục 3.2).
- Thiết kế sơ đồ quy trình trực quan (sơ đồ Mermaid và ảnh quy trình tương lai `cp5-workflow-future.png` trong `report/assets/`).
- Tham gia xây dựng bảng AI Canvas rút gọn, câu hỏi Google PAIR (Mục 6) và hoàn thiện bộ dữ liệu kiểm thử Eval Dataset (Mục 7 & asset).

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
- Thực hiện 4 cuộc phỏng vấn sâu theo đúng 3 luật The Mom Test (hỏi hành vi quá khứ, không hỏi ý tưởng tương lai, nói ít nghe nhiều), ghi chép 2 bản Interview Snapshot chi tiết trong báo cáo nhóm và lưu đầy đủ trong `report/assets/cp4-interview-snapshots.md`.
- Trích xuất insight sống còn từ người học và gia sư: học sinh bỏ cuộc vì khâu lục tìm 30 file PDF mất 45 phút, và gia sư cảnh báo tuyệt đối không để AI tự chế đề Toán mới.
- Vẽ sơ đồ Mermaid cho quy trình Before và After; tạo hình ảnh sơ đồ tương lai `cp5-workflow-future.png` lưu trong thư mục `report/assets/`.
- Hỗ trợ xây dựng 10 test cases thực tế minh họa cho 5 tiêu chí Eval lưu tại `report/assets/cp6-eval-dataset.md`.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
- `report/team/group_report.md`: Mục 3.2 (Interview Snapshots #1 & #2), Mục 4.1 & 4.2 (Sơ đồ Mermaid quy trình trước/sau), Mục 6.3 & 6.4 (AI Canvas & PAIR), Mục 7 (Tiêu chí Eval).
- File phụ lục trong assets: `report/assets/cp4-interview-snapshots.md`, `report/assets/cp5-workflow-future.png`, `report/assets/cp6-eval-dataset.md`.

**Điều mình học được từ phần nhóm:**
- Thấm thía nguyên tắc The Mom Test: lời khen của người dùng ("ý tưởng hay đấy") hoàn toàn vô giá trị; chỉ có hành vi thực tế họ đã từng làm (đã mất 45 phút lục PDF, đã nản chí bỏ cuộc) mới là bằng chứng xác thực.
- Nhận thức rõ sự khác biệt giữa Augment (hỗ trợ) và Automate (tự động hóa hoàn toàn): trong giáo dục, AI chỉ nên đóng vai trò trợ lý giảm tải việc chân tay, còn việc đọc hiểu và giải toán bắt buộc phải do con người tự rèn luyện.
