# Nguồn tham khảo cho 5 vấn đề CP1–CP2

Ngày kiểm tra: **09/11/2026 (GMT+7)**. Người dùng cung cấp 5 mô tả; phần này bổ sung số liệu từ nguồn sơ cấp đã mở kiểm tra.

Đây là **desk research**, không phải log vận hành, phỏng vấn hoặc trải nghiệm đã đo của học viên. Con số nghiên cứu, thông số sản phẩm và target đề xuất là ba loại khác nhau. Các nguồn dưới đây hỗ trợ chọn vấn đề và phản biện; không thay thế bước kiểm chứng với người thật ở CP4.

## 1. Cày giờ trong cộng đồng học trực tuyến

**[S1] [Study Together — FAQ & Rules](https://www.studytogether.com/faq).** Trang không ghi ngày cập nhật. Điều 18 cấm farming giờ và thống kê học phi thực tế. Cơ chế auto-accountability nhắc lại mục tiêu sau **2 giờ**, chuyển sang AFK nếu không phản hồi sau **10 phút**; FAQ nói cơ chế này không áp dụng cho phòng camera/chia sẻ màn hình. Đây là thông số quy trình của một cộng đồng, **không phải tỷ lệ gian lận hoặc thời gian xử lý report**.

**[S2] [StudyStream — Your stats, hours, rank and badges](https://help.studystream.live/hc/help/articles/1791807619-your-stats-hours-rank-and-badges).** Cập nhật **14/10/2026**. Giờ được tính từ lúc vào đến lúc rời phòng, kể cả nghỉ và tắt camera; bảng xếp hạng cập nhật mỗi **5 phút**. Vì vậy, thời gian trong phòng không đồng nghĩa thời gian học tập chủ động. Việc nghỉ vẫn có thể hợp lệ theo chính sách riêng của nền tảng này.

**Giới hạn và thay đổi đề xuất:** Chưa tìm được số liệu sơ cấp về tỷ lệ người treo máy hoặc số giờ moderator mất mỗi tuần. Không khẳng định “nhiều người gian lận” bằng hai nguồn trên. Thu hẹp pain thành **xác minh phiên bị báo cáo theo nội quy đã công bố**; tránh kết luận người ít chuyển động hoặc tắt camera là gian lận. Phương án Rule/check-in đã tồn tại và phải được so sánh trước khi chọn giải pháp phức tạp hơn.

## 2. Soạn bộ đề từ tài liệu mới

**[S3] [Naqvi và cộng sự — ChatGPT In Assessment (PAFMJ)](https://www.pafmj.org/PAFMJ/article/view/12930), [PDF gốc](https://www.pafmj.org/PAFMJ/article/download/12930/7944/178551).** Công bố **30/10/2026**, nghiên cứu tại Pakistan trong **02–08/2024**. Hai giảng viên soạn **50 MCQ**; **100 sinh viên y năm cuối** làm bộ người soạn và bộ ChatGPT. Thời gian tạo: **205 phút bởi người**, **25 phút bởi ChatGPT**. Phương pháp nói không review/lọc câu hỏi bởi chuyên gia trước khi thi.

**Giới hạn và thay đổi đề xuất:** Đây là một nghiên cứu giáo dục y khoa, không phải baseline đào tạo nội bộ. **25 phút không phải thời gian hoàn tất bộ đề đã duyệt.** Dùng số liệu như tham khảo về khâu tạo câu hỏi; metric của candidate phải tính cả review, sửa, kiểm đáp án và độ phủ nội dung. Không suy ra chất lượng tương đương chỉ từ kết quả chưa có khác biệt thống kê.

## 3. Kẹt khi debug và tìm thông tin

**[S4] [Alaboudi & LaToza — An Exploratory Study of Debugging Episodes](https://arxiv.org/abs/2105.02162).** Nghiên cứu **2021** quan sát **11 lập trình viên chuyên nghiệp**, **15 phiên livestream**, tổng **30 giờ**. Tác giả ghi nhận một số đợt debug dài hơn **100 phút**; nhiều đợt ngắn hơn vài phút. Mẫu nhỏ, không riêng sinh viên hoặc ban đêm.

**[S5] [Stack Overflow Developer Survey 2022](https://survey.stackoverflow.co/2022/#professional-developers-productivity-impacts).** Mục thời gian tìm câu trả lời có **36.198 phản hồi**. Báo cáo tóm tắt **62%** dành trên **30 phút/ngày**, **25%** trên **1 giờ/ngày**; câu hỏi tính cả tự tìm, hỏi đồng nghiệp và chờ trả lời. Tổng khảo sát là 73.268 người, không phải cỡ mẫu của riêng mục này.

**Giới hạn và thay đổi đề xuất:** Hai nguồn hỗ trợ pain debug/tìm thông tin, chưa chứng minh ban đêm khó hơn hoặc Google/Stack Overflow luôn trả lời chung chung. Không có tỷ lệ bỏ dở tính năng do bug từ những nguồn này. Candidate nên đo **thời gian từ lỗi tái hiện được đến giả thuyết nguyên nhân được kiểm chứng**, phân biệt thời gian tìm thông tin và thời gian thử sửa.

## 4. Phát hiện muộn sự cố tài nguyên VPS

**[S6] [Cloudflare — Details of the outage on July 2, 2019](https://blog.cloudflare.com/details-of-the-cloudflare-outage-on-july-2-2019/).** Postmortem của đơn vị vận hành: một regex trong WAF gây cạn CPU và gián đoạn **27 phút**. Cảnh báo PagerDuty đầu tiên đến **3 phút** sau triển khai. Đây là hệ thống lớn và lỗi cấu hình, **không phải một VPS nhỏ quá tải do khung giờ vàng**; nguồn cũng là tín hiệu phản bác nhận định “chỉ phát hiện khi user than phiền”.

**[S7] [DigitalOcean — Monitoring Quickstart](https://docs.digitalocean.com/products/monitoring/getting-started/quickstart/).** Trang ghi kiểm tra **06/10/2026**. Có cảnh báo CPU/RAM/disk theo ngưỡng và khoảng duy trì **5, 10, 30 phút hoặc 1 giờ**; thông báo qua email/Slack. Tài liệu gợi ý ngưỡng khởi đầu **70%**, cần điều chỉnh theo dịch vụ. Đây là cấu hình sản phẩm, không phải baseline sự cố hoặc ngưỡng an toàn phổ quát.

**Giới hạn và thay đổi đề xuất:** Chưa có số downtime/tháng hoặc latency của dự án học viên. Thu hẹp candidate thành **rút ngắn thời gian từ dịch vụ suy giảm đến khi quản trị viên nhận biết**. So sánh Rule + monitoring + runbook trước. Không dùng 27 phút của Cloudflare làm downtime trung bình VPS, không cam kết cảnh báo tài nguyên tự dự đoán được mọi sự cố.

## 5. Trôi thông tin và cập nhật tiến độ nhóm

**[S8] [Asana — Anatomy of Work Index 2022, công bố chính thức](https://investors.asana.com/node/6631/pdf).** Công bố **05/04/2022**; GWI khảo sát **10.624 lao động tri thức tại 7 quốc gia** trong **10/2021** theo đặt hàng Asana. Báo cáo ghi **58%** ngày làm việc dành cho điều phối công việc. Đây là dữ liệu tự báo cáo và có bối cảnh nhà cung cấp công cụ quản lý công việc.

**Giới hạn và thay đổi đề xuất:** “Điều phối công việc” rộng hơn việc hỏi tiến độ qua chat; không thể nói toàn bộ 58% là lãng phí hoặc áp dụng tỷ lệ này cho nhóm sinh viên. Candidate nên tách **thời gian gom/cập nhật trạng thái** khỏi họp ra quyết định. Đo thêm task thiếu người phụ trách/deadline; thử bảng việc chung và quy ước cập nhật trước khi chọn hỗ trợ tổng hợp văn bản.

## Cách dùng trong bản nháp

| Candidate | Bằng chứng hiện có | Điều chưa đủ để kết luận |
|---|---|---|
| 1 — Cày giờ | Nội quy và cơ chế chống AFK có thật; S1–S2 | Chưa có tỷ lệ vi phạm hoặc thời gian moderator |
| 2 — Tạo đề | Thời gian tạo 50 câu trong nghiên cứu gốc; S3 | Chưa đo quy trình tài liệu → bộ đề đã duyệt của học viên |
| 3 — Debug | Nghiên cứu quan sát và khảo sát gốc; S4–S5 | Chưa có dữ liệu cá nhân, bằng chứng riêng ban đêm hay tỷ lệ bỏ dở |
| 4 — VPS | Postmortem và cảnh báo Rule có thật; S6–S7 | Chưa có log VPS nhỏ, baseline downtime và thời gian phát hiện |
| 5 — Tiến độ nhóm | Khảo sát gốc về điều phối công việc; S8 | Chưa đo nhóm sinh viên và phần overhead riêng chat |

Các mục chưa đủ được giữ thành giả định cần kiểm chứng. Không chuyển số liệu bên ngoài thành lời kể “tôi đã mất…” hoặc điền giả kết quả phỏng vấn. Thời gian từng bước trong quy trình nháp chỉ được gắn nhãn **ước lượng kịch bản** nếu chưa có đo trực tiếp; tổng ước lượng không được gọi là baseline đã xác thực.
