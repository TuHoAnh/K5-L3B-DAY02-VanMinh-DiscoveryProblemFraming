# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: Văn Minh
- Candidate problem nhóm chọn (1 câu): Khi chuẩn bị nộp bài lab môn học, tôi muốn đối chiếu nhanh bài làm và cấu trúc thư mục của mình với toàn bộ yêu cầu rubric/checklist, để đảm bảo không bị trừ điểm oan do thiếu mục hoặc sai quy cách nộp bài.
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet

## Thành viên

| STT | Họ và tên        | MSSV        | Vai trò trong nhóm                                                        | Tài khoản GitHub |
| --: | ---------------- | ----------- | ------------------------------------------------------------------------- | ---------------- |
|   1 | Hồ Anh Tú        | 2A202603811 | Nhóm trưởng, điều phối chung, phụ trách CP3, thuyết trình demo            | TuHoAnh          |
|   2 | Nguyễn Nam Khánh | 2A202603871 | Phụ trách kiểm chứng & research (CP4), phản biện chính, thuyết trình demo | BSFactor         |
|   3 | Vũ Văn Bình      | 2A202603831 | Phụ trách quy trình & Problem Statement v0 (CP5), phản biện               | hnib1908         |
|   4 | Lê Thanh Tùng    | 2A202603819 | Phụ trách mức can thiệp AI, eval & quyết định (CP6), phản biện            | Griin-03         |

## Phân công theo checkpoint

| Checkpoint                                 | Người chính      | Người hỗ trợ                | Sản phẩm                                       |
| ------------------------------------------ | ---------------- | --------------------------- | ---------------------------------------------- |
| CP3 — Hội tụ nhóm                          | Hồ Anh Tú        | Cả nhóm (Khánh, Bình, Tùng) | Cluster, cây OST, bảng chấm điểm               |
| CP4 — Kiểm chứng                           | Nguyễn Nam Khánh | Hồ Anh Tú                   | Assumption map, snapshot hoặc survey           |
| CP4 — Research                             | Nguyễn Nam Khánh | Lê Thanh Tùng               | Bảng research có link                          |
| CP5 — Quy trình trước/sau                  | Vũ Văn Bình      |                             | Quy trình + bảng before/after                  |
| CP5 — Problem Statement v0                 | Vũ Văn Bình      | Nguyễn Nam Khánh            | Problem Statement v0                           |
| CP6 — Mức can thiệp + Problem Statement v1 | Lê Thanh Tùng    | Vũ Văn Bình                 | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định                           | Lê Thanh Tùng    |                             | 4 rủi ro + Go/Not Yet/No-Go                    |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### HoVaTen-MSSV

**Phần việc phụ trách:**

- **Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- **Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- **Điều mình học được từ phần nhóm:**

-

### HoAnhTu-2A202603811 (Nhóm trưởng)

**Phần việc phụ trách:**

- Khởi tạo và quản lý GitHub Repository của nhóm (Fork repo, cấu hình quyền Collaborator, hướng dẫn workflow nhánh).
- Chủ trì buổi thảo luận pitch và phản biện nội bộ CP3; xây dựng cấu trúc Cây Cơ hội (Opportunity Solution Tree - OST).
- Trực tiếp đóng góp đề tài được chọn làm bài toán chung của nhóm: _Rà soát checklist/rubric bài lab trước khi nộp_.
- Trực tiếp thực hiện phỏng vấn người dùng thật theo chuẩn The Mom Test tại lớp (CP4) và nghiên cứu giải pháp Pre-commit hooks/Linter.
- Thiết kế sơ đồ luồng quy trình Hiện tại (As-Is) và Tương lai (To-Be) 2 tầng (Rule + LLM) kèm bước Human-in-the-loop (CP5).
- Chủ trì xây dựng bộ tiêu chí đánh giá (Eval), phân tích rủi ro và xác lập Ngưỡng dừng (Stop condition) cho quyết định Go/No-Go (CP6).
- Đảm nhận thuyết trình và trả lời các câu hỏi thắc mắc của lớp, giúp team được cộng điểm

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Đóng góp **Problem Card #2** (Rà soát checklist/rubric) đạt điểm tuyệt đối 35/35 ở vòng chấm Shortlist; chủ động đề xuất tích hợp bài toán xác định yêu cầu của bạn Bình (#10) vào làm khâu tiền xử lý để tối ưu sự đồng thuận của nhóm.
- Tiến hành 01 buổi phỏng vấn trực tiếp học viên nhóm 02 tại lớp theo đúng 3 nguyên tắc The Mom Test, trích xuất raw quote và insight then chốt: _Áp lực thời gian khiến học viên dễ bỏ qua khâu đối chiếu và có nguy cơ bị điểm 0 oan_.
- Soạn thảo bản thảo sơ đồ quy trình tương lai To-Be dạng Mermaid, phân định rõ ràng giữa tầng 1 (Rule-based check định dạng file, regex tên, số từ) và tầng 2 (LLM Semantic Audit).
- Viết bản nháp và hoàn thiện **Problem Statement v0 & v1**; thiết lập ranh giới cứng (Boundary: AI chỉ có quyền Read & Warn, cấm tự ý sửa file hay tự push code).
- Định nghĩa bộ Benchmark 10 bài lab mẫu và chỉ số Semantic Precision $\ge 85\%$ để ngăn chặn rủi ro False Positive gây hoang mang cho người dùng.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`:
  - Phần CP3 (Hội tụ nhóm): Bảng Pitch Candidate #5, sơ đồ cây OST và bảng chấm điểm Shortlist.
- `report/individual/2A202603811_HoAnhTu.md`: Báo cáo cá nhân đầy đủ từ CP1 đến CP7.
- Commits trên repo:
  - `feat: complete CP1 and CP2 individual report`
  - `feat(team): initialize group report structure and finalize CP3 convergence`

**Điều mình học được từ phần nhóm:**

- **Tư duy Problem-first đè bẹp Solution-first:** Trước khi làm lab, tôi thường có xu hướng nghĩ ngay đến việc xây AI Agent tự động hóa toàn bộ. Quá trình làm việc cùng nhóm và phản biện qua cây OST đã chứng minh rằng: Một quy trình tốt bắt đầu từ việc chỉ ra đúng bước nghẽn (bottleneck) và dùng giải pháp đơn giản nhất đủ tốt (Rule kết hợp Workflow nhỏ gọn), chứ không phải lạm dụng AI phức tạp.
- **Sức mạnh của phản biện đa chiều:** Nhờ câu hỏi chất vấn sâu sắc của bạn Bình về rủi ro "báo nhầm" (False Positive), tôi nhận ra rằng trong môi trường giáo dục sát deadline, tính chính xác và sự kiểm soát của con người (Human-in-the-loop) quan trọng hơn nhiều so với việc tự động hóa hoàn toàn.
- **Kỹ năng điều phối Leader:** Học cách dung hòa quan điểm khác biệt, lắng nghe và tích hợp ý tưởng của các thành viên (như việc ghép bài của Bình vào bài của mình) để toàn đội có chung một mục tiêu và sở hữu chung sản phẩm (shared ownership).

### LeThanhTung-2A202603819

**Trạng thái ngày 09/11/2026:** có CP1–CP2; đã chuẩn bị thêm tài liệu cá nhân cho hướng kiểm tra bài lab trước khi nộp. Chưa có ghi chép phỏng vấn, câu hỏi pitch trực tiếp hoặc quyết định chung để bổ sung từ phía tôi.

**Phần việc đã chuẩn bị:**

- CP1: đưa ra 5 vấn đề về cộng đồng học tập, tạo đề, debug, VPS và tiến độ nhóm.
- CP2: chuẩn bị 3 card về tạo đề, tiến độ nhóm và gian lận thời gian học, kèm 3 quy trình nháp. Chọn gian lận thời gian thay cho VPS vì hiểu vấn đề này hơn; thời gian từng bước còn cần đo.
- Cách dùng AI trong quá trình chuẩn bị được ghi ở mục 5 của báo cáo cá nhân.
- CP3: nhờ đối chiếu bài của Tú, Khánh và Bình với README; yêu cầu chuẩn bị demo cho hướng kiểm tra bài lab trước khi nộp.
- CP4: chuẩn bị bảng giải pháp hiện có và các giả định cần kiểm chứng; chưa thực hiện phỏng vấn/survey ngoài nhóm.
- CP5–CP6: chuẩn bị slide/demo HTML để thuyết trình, quy trình giả thuyết, giá trị tính năng, kế hoạch benchmark, lộ trình và bốn rủi ro. Có AI hỗ trợ; các ngưỡng đo là đề xuất, chưa có kết quả chạy.
- CP6: bổ sung trực tiếp mục 6–8 trong báo cáo nhóm: ma trận, so sánh bốn mức, đề xuất Rule, v1, năm tiêu chí đánh giá, bốn rủi ro và đề xuất Not Yet. Bản đề xuất có AI hỗ trợ soạn; nhóm cần tự kiểm, chỉnh và chốt theo quy định.

**Sản phẩm hiện có:**

- [Báo cáo cá nhân — CP1, CP2, nhật ký tham gia, dùng AI và bản nháp CP7](report/individual/2A202603819_LeThanhTung.md).
- [Memo nguồn công khai cho 5 vấn đề](report/assets/cp1-2-evidence-research.md).
- [Ghi chú đóng góp CP3–CP6 cho hướng LabCheck](report/assets/cp3-6-le-thanh-tung-labcheck.md): cơ sở chọn hướng, research, quy trình, benchmark và rủi ro. Nội dung chuyển từ phần slide/demo đã chuẩn bị; không thay cho quyết định nhóm.
- [Phần CP6 đề xuất trong báo cáo chung](report/team/group_report.md#6-mức-can-thiệp-ai-cp6), gồm cả v1 và quyết định tại mục 7–8.

**Đóng góp vào phần nhóm và điều học được:**

- Có tài liệu chuẩn bị để nhóm sử dụng khi thảo luận CP3–CP6. Bảng pitch chung hiện có 3 candidate của tôi ở dòng 7–9.
- Phần cần làm rõ trong bản nháp cá nhân: kiểm cấu trúc không chứng minh chất lượng; phải đo cả công đọc/sửa cảnh báo và lỗi còn sót trước khi quyết định cần AI.
- CP7 có bản nháp do AI hỗ trợ; cần tự viết lại theo yêu cầu đề bài, không ghi nhận đây là reflection tự viết đã hoàn tất.

### Nguyễn Nam Khánh-2A202603871

**Phần việc phụ trách:**

- Phụ trách chuẩn bị kiểm chứng và research ở CP4; tham gia pitch, phản biện và thảo luận chọn candidate ở CP3.
- Hỗ trợ thảo luận quy trình, Problem Statement, mức can thiệp và quyết định của nhóm.

- **Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):
  - Chuẩn bị 3 Problem Card cá nhân và quy trình nháp; đưa vào bảng pitch chung.
  - Phản biện bài toán tổng hợp deadline bằng câu hỏi.
  - Chuẩn bị assumption map cho bài toán đối chiếu rubric/checklist trước khi nộp.
  - Research checklist Notion/giấy và script qua pre-commit, đối chiếu khả năng xử lý, hạn chế và bài học cho nhóm.
  - Góp ý thu hẹp phạm vi vào thiếu mục bắt buộc và sai quy cách; ưu tiên cách làm đơn giản, chi phí thấp trước khi cân nhắc AI.

- **Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):
  - [Báo cáo nhóm](report/team/group_report.md): mục 2.1, candidate #1–#3; mục 3.1–3.3, assumption map, snapshot và research.

- **Điều mình học được từ phần nhóm:**
  - Cần xác định actor và bottleneck cụ thể, đồng thời so sánh với giải pháp có sẵn để tránh làm phức tạp vấn đề.
  - Phản biện giúp làm rõ giá trị của giải pháp; script hoặc checklist có thể đã đủ cho các quy tắc cố định.
  - Cần đo cả thời gian và lỗi còn sót, phân biệt giả định với bằng chứng thực tế; quyết định Not Yet giúp nhóm xác định điều phải kiểm chứng trước khi triển khai.
