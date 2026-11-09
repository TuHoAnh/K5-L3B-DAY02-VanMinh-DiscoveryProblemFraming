# Ghi chú đóng góp cá nhân CP3–CP6 — Lê Thanh Tùng

- MSSV: **2A202603819**; nhóm Văn Minh.
- Ngày cập nhật: **09/11/2026**.
- Nguồn nội dung: phần chuẩn bị slide/demo LabCheck theo yêu cầu của tôi, có AI hỗ trợ tổng hợp.
- Trạng thái: tài liệu chuẩn bị để nhóm thảo luận. Chưa có phỏng vấn, số đo baseline, kết quả benchmark hoặc quyết định chung trong tài liệu này.
- Liên kết: [báo cáo cá nhân](../individual/2A202603819_LeThanhTung.md), [báo cáo nhóm](../team/group_report.md).

## 1. CP3 — Cơ sở đề xuất hướng chung

| Báo cáo | Vấn đề liên quan | Phần có thể đưa vào cùng phạm vi |
|---|---|---|
| [Hồ Anh Tú](../individual/2A202603811_HoAnhTu.md), card #2 | Đối chiếu bài với rubric/checklist trước khi nộp. | Phát hiện yêu cầu còn thiếu trong một bài lab. |
| [Nguyễn Nam Khánh](../individual/2A202603871_NguyenNamKhanh.md), card #2 | Đổi tên file, điền và kiểm tra thông tin. | Kiểm quy cách tệp và các mục thông tin bắt buộc. |
| [Vũ Văn Bình](../individual/2A202603831_VuVanBinh.md), card #1 | Xác định yêu cầu cuối cùng từ nhiều kênh. | Xác nhận đúng phiên bản yêu cầu trước khi đối chiếu bài. |
| [Lê Thanh Tùng](../individual/2A202603819_LeThanhTung.md), card #3 | Xác minh report gian lận giờ học theo nội quy. | Là phương án cá nhân tôi muốn trao đổi trước; không ép ghép vào vấn đề rà bài lab. |

**Candidate dùng để chuẩn bị demo**, giữ nguyên nội dung đã yêu cầu:

> Khi chuẩn bị nộp một bài lab, học viên muốn xác định bài còn thiếu yêu cầu nào và có sai quy cách nộp hay không, để sửa kịp trước deadline và tránh mất điểm do bỏ sót.

Điểm thuận lợi của hướng này là actor và đầu ra rõ, có thể giới hạn trong một bài, dùng tài liệu công khai và so sánh với checklist. Hướng gian lận giờ học cần tiếp cận quản trị viên, thông tin phiên học và quy tắc xác minh; các dữ liệu này chưa có trong phần chuẩn bị của tôi. Đây là lập luận đề xuất, không phải kết quả chấm điểm hay đồng thuận đã diễn ra trong nhóm.

**Giới hạn phạm vi:** rà yêu cầu và quy cách nộp; không mở rộng sang quản lý toàn bộ deadline, tự viết bài, chấm điểm hay tự nộp. Bảng điểm shortlist, OST và câu hỏi pitch thực tế cần nhóm ghi tại CP3, không lấy nhận xét AI thay cho hoạt động trực tiếp.

## 2. CP4 — Research và việc cần kiểm chứng

### Giải pháp hiện có

| Công cụ / cách làm | Giải quyết bước nào? | Giới hạn cần so sánh | Nguồn |
|---|---|---|---|
| Checklist thủ công | Người học đối chiếu từng yêu cầu với bài làm. | Phụ thuộc checklist đúng phiên bản và việc người học kiểm từng mục. | [README](../../README.md), [CHECKPOINTS](../../CHECKPOINTS.md), [SUBMISSION](../../SUBMISSION.md). |
| Script + GitHub Actions, có thể kết hợp markdownlint | Script kiểm các quy tắc đã cấu hình; Actions chạy theo sự kiện; markdownlint kiểm định dạng Markdown. | Cần tính công viết và bảo trì rule; có heading hoặc file không chứng minh nội dung đạt rubric. | [GitHub Docs](https://docs.github.com/en/actions/how-tos/write-workflows/choose-when-workflows-run/trigger-a-workflow), [markdownlint](https://github.com/DavidAnson/markdownlint). |
| Gemini với prompt và bộ tệp cố định | Đối chứng đề xuất cho phần đọc hiểu nội dung và tìm dẫn chứng. | Phải kiểm giá trị đầu ra, không coi đúng schema là đúng nội dung; chưa chạy đối chứng này. | [Gemini structured outputs](https://ai.google.dev/gemini-api/docs/structured-output). |

Các nguồn là desk research cho bản demo, không phải bằng chứng LabCheck hiệu quả. Bài Tú tự báo cáo 25–30 phút rà bài; số của Khánh nói về chuẩn bị file, còn Bình ghi rõ các thời gian là ước tính AI. Không lấy trung bình những số này làm baseline.

### Giả định cần kiểm chứng trước

| Giả định | Loại rủi ro | Cách kiểm chứng đề xuất |
|---|---|---|
| Người học thường bỏ sót yêu cầu dù đã đọc hướng dẫn. | Value | Hỏi 2–3 học viên ngoài nhóm về lần nộp gần nhất; xin xem ví dụ đã ẩn thông tin riêng nếu họ đồng ý. |
| Đối chiếu yêu cầu là bước tốn công, không chỉ do bài chưa làm xong. | Value | Quan sát một lần tự kiểm; tách thời gian đọc, tìm file, đối chiếu, sửa và chờ. |
| Người học phân biệt được “đã kiểm cấu trúc” với “nội dung đạt yêu cầu”. | Usability | Cho xem kết quả mẫu và yêu cầu họ giải thích còn mục nào phải tự kiểm. |
| Rule đủ xử lý phần lớn lỗi quy cách trong phạm vi một lab. | Feasibility | Chạy trên các snapshot có nhãn; so sánh lỗi phát hiện và lỗi còn sót. |
| Có thể dùng bài nộp đúng quyền và duy trì bộ yêu cầu theo phiên bản. | Viability | Xác nhận quyền sử dụng dữ liệu, người cập nhật và công bảo trì trước pilot. |

**Chưa thực hiện phỏng vấn/survey.** Không điền Interview Snapshot bằng người dùng giả. Khi hỏi, ưu tiên hành vi đã xảy ra: “Lần gần nhất bạn rà bài thế nào?”, “Bạn đã bỏ sót mục gì?”, “Bạn phát hiện khi nào?”, “Mất bao lâu?”, “Checklist hiện có giúp được đến đâu?”. Cần ghi cả trường hợp checklist đã đủ hoặc người học không gặp vấn đề.

## 3. CP5 — Quy trình dùng để giải thích demo

Đây là quy trình giả thuyết để chuẩn bị thảo luận, chưa phải quy trình được quan sát và bấm giờ.

```text
HIỆN TẠI — học viên thực hiện
Đọc nguồn yêu cầu → Mở bài/tệp → Đối chiếu từng mục → Sửa và kiểm lại → Tự nộp
                                ^ bottleneck giả thuyết

ĐỀ XUẤT
Người học xác nhận nguồn yêu cầu và phiên bản
 → Cung cấp snapshot bài được phép kiểm
 → Rule kiểm tên file, vị trí, mục cấu trúc bắt buộc [demo hiện có]
 → Đọc hiểu nội dung, dẫn chứng [con người; AI là phương án thử sau]
 → Người học xem từng cảnh báo, sửa và kiểm lại
 → Người học tự nộp

Thiếu tệp / nguồn mâu thuẫn / không đủ căn cứ
 → Báo “chưa kiểm được / cần người kiểm”
 → Quay về checklist và nguồn gốc, hỏi coach khi cần
```

| Bước hiện tại | Actor | Input → Output | Thời gian |
|---|---|---|---|
| Đọc yêu cầu | Học viên | README, rubric, hướng dẫn nộp → danh sách yêu cầu áp dụng. | Chưa đo. |
| Mở bài và tệp | Học viên | Snapshot bài → các phần cần đối chiếu. | Chưa đo. |
| Đối chiếu | Học viên | Yêu cầu + bài → các điểm thiếu/sai/cần xác nhận. | Chưa đo; bottleneck giả thuyết. |
| Sửa và kiểm lại | Học viên | Các điểm cần xử lý → bài đã sửa, mục chưa giải quyết. | Chưa đo; tính cả vòng sửa lại. |
| Tự nộp | Học viên | Bài đã rà → bản nộp và xác nhận nộp. | Chưa đo; tách khỏi thời gian kiểm trong benchmark. |

**Before/after dự kiến:** từ việc đối chiếu thủ công sang có danh sách phát hiện kèm nguồn. Chưa có số đo thời gian hoặc số lỗi trước/sau; mục tiêu đề xuất là giảm ít nhất 30% trung vị thời gian rà và sửa, không tăng lỗi còn sót. Thời gian đo từ mở yêu cầu đến hoàn tất sửa/kiểm lại, tính cả thời gian chờ công cụ và xử lý cảnh báo sai.

**Các lỗ hổng cần nhóm xử lý khi viết v0/v1:** xác định đúng actor; chốt một lab và phiên bản yêu cầu; đo baseline; phân biệt kiểm cấu trúc với kiểm chất lượng; ghi rõ công cụ không tự sửa, tự nộp hay cấp điểm. Job Story ở mục 1 là đầu vào; tài liệu này không công bố v0/v1 đã được nhóm thông qua.

## 4. CP6 — Mức can thiệp và giá trị tính năng

| Mức | Phương án để thử | Khi nào đủ / cần thêm? |
|---|---|---|
| No AI | Một checklist có nguồn và phiên bản. | Đủ nếu người học kiểm nhanh, ít bỏ sót; là đối chứng bắt buộc. |
| Rule | Kiểm các điều kiện cấu trúc đã định nghĩa. | Là phạm vi demo hiện có; có thể đủ với lỗi tên tệp, vị trí và thiếu mục. |
| Workflow | Rule trước, AI gợi ý cho nội dung tự do, người học kiểm sau. | Chỉ đáng thử nếu Rule chưa đủ và phần AI có lợi ích đo được sau khi tính công review. |
| Agent | Công cụ tự chọn nhiều bước và hành động. | Chưa có nhu cầu rõ; quy trình này đang có đầu vào và các bước cố định. |

Mức mơ hồ thấp ở tên file/cấu trúc, cao hơn ở chất lượng nội dung; độ phức tạp được giới hạn trong một bài. Vì vậy, không mặc định phải dùng AI cho toàn bộ bài toán. Chưa có quyết định mức can thiệp chung của nhóm.

| Tính năng đề xuất | Giá trị cần kiểm chứng | Chỉ số |
|---|---|---|
| Kiểm tệp và cấu trúc | Thấy lỗi quy cách trước khi nộp. | Lỗi cấu trúc phát hiện đúng và còn sót. |
| Đối chiếu yêu cầu có dẫn nguồn | Biết cảnh báo dựa vào đâu, sửa ở mục nào. | Độ đúng của finding và nguồn dẫn. |
| Phân loại “thiếu / cần kiểm” | Tránh hiểu nhầm công cụ đã xác nhận toàn bộ bài đạt. | Số lần kết luận đạt khi thiếu căn cứ; khả năng người học hiểu trạng thái. |
| Người học kiểm lại | Giữ quyết định sửa và nộp ở người làm bài. | Lỗi còn lại sau khi xử lý cảnh báo; tổng thời gian. |

### Benchmark đã chuẩn bị trong slide — chưa chạy

- **Bốn điều kiện:** A checklist thủ công; B script + Actions; C Gemini với prompt cố định; D Rule + AI gợi ý có nguồn + người học kiểm. D đầy đủ còn là kế hoạch; demo HTML hiện chỉ có rule.
- **Bộ 40 snapshot dự kiến:** 10 đủ cấu trúc, 10 lỗi tệp, 10 thiếu nội dung, 10 mơ hồ/mâu thuẫn/gây nhiễu. Hai người gán nhãn độc lập và giải quyết bất đồng.
- **Tách dữ liệu:** 2 mẫu mỗi loại để phát triển = 8; 8 mẫu mỗi loại giữ lại để đánh giá = 32. Tách theo bài gốc; không để các biến thể cùng bài lọt cả hai tập. Không chỉnh rule/prompt theo tập giữ lại rồi báo là kết quả độc lập.
- **Offline:** so B/C/D trên cùng dữ liệu; ghi riêng cấu trúc và nội dung, phạm vi không kiểm được; chạy LLM 3 lần để xem dao động. So D với bản chỉ Rule để biết AI có thêm giá trị gì.
- **Pilot dự kiến:** 12 học viên ngoài nhóm × 4 điều kiện = 48 phiên. Mỗi người dùng bốn task khác nhau, tương đương; xoay thứ tự công cụ và task. Người chấm lỗi cuối không biết công cụ đã dùng.
- **Mục tiêu đề xuất:** recall lỗi bắt buộc ≥95%; precision cảnh báo ≥90%; trung vị tổng thời gian giảm ≥30% so với A và so thêm B/C; lỗi còn sót không tăng. Báo cả tử số, mẫu số và loại lỗi; mẫu nhỏ không phải bảo đảm độ chính xác cho mọi môn.
- **Trường hợp mơ hồ:** không tự kết luận toàn bộ bài đạt; báo tỷ lệ chuyển người kiểm và mức bao phủ để tránh việc từ chối mọi trường hợp.

### Bốn rủi ro và điều kiện dừng đề xuất

| Rủi ro | Mức nhận định ban đầu | Vấn đề cần theo dõi | Cách giảm / tiêu chí quyết định |
|---|---|---|---|
| Value | Cao — chưa kiểm chứng | Làm xong công cụ nhưng checklist đã đủ tốt. | Phỏng vấn và đo A/B trước; nếu D không cải thiện so với B sau khi tính công review thì giữ Rule/checklist. |
| Usability | Cao — chưa thử người dùng | Người học hiểu “đủ cấu trúc” thành “đạt toàn bài”; cảnh báo quá nhiều. | Ghi trạng thái rõ, dẫn nguồn, ưu tiên lỗi quan trọng; có lần xác nhận đạt khi thiếu căn cứ thì sửa trước khi mở rộng. |
| Feasibility | Trung bình — rule có demo, phần đọc hiểu chưa đánh giá | Bỏ sót yêu cầu, dẫn nguồn sai, rubric thay đổi, chỉ thị gây nhiễu trong bài. | Khóa phiên bản yêu cầu; đối chiếu nhãn chuẩn; không chạy code/chỉ thị trong bài nộp; không đạt recall/precision đề xuất thì tiếp tục sửa và giữ người kiểm. |
| Viability | Chưa rõ — chưa đo công vận hành | Dữ liệu riêng tư, quyền sử dụng, chi phí API và công bảo trì. | Rule chạy cục bộ; phần gửi dịch vụ ngoài phải được chủ dữ liệu cho phép; đo chi phí/lượt và công cập nhật; chưa rõ quyền thì chưa đưa dữ liệu đó vào pilot. |

**Lộ trình đề xuất 14 ngày:** ngày 1–2 chốt yêu cầu và nhãn phát triển; ngày 3–5 làm rule/giao diện; ngày 6–9 thử phần đọc hiểu và đánh giá tập giữ lại; ngày 10–14 pilot, tổng hợp kết quả và quyết định. Đây là kế hoạch để nhóm cân nhắc, chưa phải phân công đã được nhận.

**Căn cứ hiện tại:** có bản demo và kế hoạch đánh giá, chưa đủ dữ liệu để kết luận Go triển khai rộng. Nếu nhóm chọn thử nhỏ thì phải ghi rõ phần nào được thử, ai kiểm, dữ liệu nào được phép dùng và các ngưỡng ở trên; không báo các mục tiêu như kết quả đã đạt.

## 5. Phần còn cần người thật bổ sung

- Câu hỏi phản biện tôi thực sự đặt/nhận trong CP3 và thay đổi sau đó.
- Phỏng vấn/survey ngoài nhóm, có thời điểm, cách hỏi, tín hiệu xác nhận và phản bác.
- Baseline quan sát thực tế; kết quả benchmark nếu được thực hiện.
- Lập luận và quyết định v0/v1 của nhóm trong báo cáo chung.
- Reflection do tôi tự viết theo quy định CP7; bản AI hỗ trợ trong báo cáo cá nhân chỉ để tham khảo.
