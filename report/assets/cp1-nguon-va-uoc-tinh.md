# CP1 — Ghi chú nguồn và cách ước tính

### Nguồn tham khảo cho từng problem

Các nguồn dưới đây đã được AI mở và đọc ngày 09/11/2026; học viên cần tự mở, kiểm tra trước khi sử dụng trong bài nộp. Nguồn chỉ hỗ trợ nội dung ghi tại bảng, không chứng minh các phút ước tính bên dưới.

| Problem | Dữ kiện/nhận định từ nguồn công khai | Phạm vi và giới hạn |
|---|---|---|
| #1 — Yêu cầu bài tập nhiều kênh | [S1 — Office for Students, NSS 2025](https://www.officeforstudents.org.uk/data-and-analysis/national-student-survey-data/nss-data-archive/nss-2025-results/): tỷ lệ phản hồi thuộc hai mức tích cực nhất là **79,5%** về truyền đạt thay đổi trong giảng dạy và **78,1%** về độ rõ ràng của tiêu chí chấm. | Bối cảnh giáo dục đại học tại Anh và các vùng thuộc UK trong khảo sát. Đây không phải tỷ lệ sinh viên bỏ sót bài tập hoặc thời gian tìm thông tin; không chứng minh nguyên nhân là nhiều kênh và không suy rộng sang lớp của học viên. |
| #2 — Tổng hợp bài nhóm | [S2 — Almazovaite, Cohn và Kumar, Frontiers in Education, 2024](https://www.frontiersin.org/journals/education/articles/10.3389/feduc.2024.1480929/full): nghiên cứu định tính phỏng vấn **18 sinh viên thuộc 10 học phần** tại một trường liberal arts ở Mỹ, ghi nhận vai trò của công nghệ trong phối hợp, chia sẻ ghi chú và làm việc không đồng thời. | Cỡ mẫu mô tả nghiên cứu, không phải số người gặp lỗi ghép bài. Nguồn hỗ trợ bối cảnh phối hợp nhóm, không cung cấp tỷ lệ trùng/mâu thuẫn hoặc phút tổng hợp. |
| #3 — Địa bàn quầy thuốc | [S3 — Google Maps Help](https://support.google.com/maps/answer/1628031?hl=en): chức năng Measure distance đo khoảng cách đường thẳng giữa các điểm, hiển thị km hoặc mile. | Xác nhận công cụ kiểm tra thủ công có sẵn. **3 km là chính sách học viên cung cấp**, không phải tiêu chuẩn ngành hay kết luận của Google; chưa có dữ liệu công khai được kiểm chứng về thời gian xét duyệt mạng lưới này. |
| #4 — Lịch sử sửa chữa | [S4 — IFS Cloud 23R2, Historical Data](https://docs.ifs.com/ifsclouddocs/23r2/PerfMaintEng/AboutHistoricalData.htm), mục Serial Fault History và Maintenance Order History: hệ thống lưu lỗi, hành động sửa chữa và thông tin công việc đã thực hiện. | Đây là ví dụ hệ thống quản lý bảo trì có lưu lịch sử, không phải khảo sát tiệm sửa gia dụng Việt Nam; không có số phút tìm hồ sơ hoặc tỷ lệ khách quay lại. |
| #5 — So sánh phòng trọ | [S5 — Nhà Tốt, 13/03/2026](https://www.nhatot.com/kinh-nghiem/cac-chi-phi-khi-o-tro.html): liệt kê các khoản thuê, điện/nước, dịch vụ/quản lý, gửi xe; phân biệt chi phí ban đầu và hằng tháng. | Bài hướng dẫn của nền tảng thương mại, không phải khảo sát đại diện; dùng để lập danh sách khoản cần hỏi, không dùng như bằng chứng về thời gian tìm trọ hoặc tỷ lệ tin thiếu phí. |

### Ước tính ban đầu để thiết kế phép đo — chưa phải dữ liệu thật

Các số dưới đây được AI dựng từ khối lượng thao tác giả định, không lấy từ các nguồn S1–S5. Chúng giúp hình dung quy mô công việc; sau khi bấm giờ phải thay bằng số thực tế, kể cả khi số thực tế thấp hơn nhiều. Không giả định số người gặp, tần suất hoặc tỷ lệ sai khi chưa thu thập dữ liệu.

| Problem | Kịch bản và cách cộng thời gian giả định | Tổng mô phỏng | Cách thay bằng số thật |
|---|---|---:|---|
| #1 | Một bài có thông tin trên LMS, chat và ghi chú lớp: đọc đề 3 + tìm tin 5 + đọc ghi chú 2 + đối chiếu 7 + soạn câu hỏi 3 + checklist 2 phút. | **22 phút/bài** | Bấm giờ từng bước trên một bài gần nhất; lưu nguồn yêu cầu. Tách thời gian chờ trả lời. |
| #2 | Một báo cáo nhóm 4 người, khoảng 12–15 trang, đã đủ bản nháp: tập hợp 5 + ghép 8 + đọc chéo 25 + trao đổi 10 + cập nhật 15 + kiểm cuối 7 phút. | **70 phút/bài**, trong đó đọc chéo **25 phút** | Dùng lịch sử chỉnh sửa kết hợp nhật ký thời gian; ghi độ dài, số thành viên và số lỗi để so sánh bài tương đương. |
| #3 | Một quầy mới, danh sách giả định 10 quầy đã nhận: tiếp nhận 1 + kiểm thông tin 2 + xác nhận vị trí 2 + đo 10 khoảng cách × 0,5 + quyết định 1 + lưu 1 phút. | **12 phút/hồ sơ**, đối chiếu khoảng cách **5 phút** | Đo một hồ sơ thật với danh sách hiện có; 10 quầy và 0,5 phút/lần đo chỉ là giả định. Không cộng giờ chờ bổ sung thông tin. |
| #4 | Một ca quay lại: hỏi thông tin nhận diện 3 + tìm phiếu/tin nhắn cũ 6 + đọc lại hạng mục đã sửa 3 phút. Không gồm chẩn đoán hoặc sửa máy. | **12 phút/ca tra cứu** | Quan sát một ca có thật; ghi cách lưu hồ sơ và thời gian tìm. Không coi tổng này là thời gian sửa chữa. |
| #5 | So sánh 10 tin và liên hệ 5 chủ trọ: đọc 10 × 3 + hỏi thông tin 5 × 4 + lập bảng so sánh 15 phút. | **65 phút/lượt so sánh** | Ghi thời gian thao tác, số tin/số cuộc liên hệ thực tế; không gồm chờ phản hồi, đi xem phòng hoặc toàn bộ thời gian tìm được chỗ ở. |

**Lý do đưa vào danh sách:**

- #1: Thông tin có thể thay đổi qua nhiều kênh; cần phân biệt yêu cầu cũ và yêu cầu còn hiệu lực.
- #2: Các phần riêng có thể hoàn thành nhưng chưa thống nhất khi ghép; cần xác định lượng công việc sửa thực sự phát sinh.
- #3: Người phụ trách cần đối chiếu vị trí quầy mới với các quầy đã nhận để áp dụng chính sách khoảng cách 3 km đường chim bay; quy tắc rõ nhưng thời gian xử lý và sai sót thực tế cần được đo.
- #4: Lịch sử sửa chữa thiếu hoặc khó tìm có thể khiến kỹ thuật viên phải hỏi lại; cần xác minh với người làm nghề.
- #5: Tin phòng trọ không cùng cấu trúc và có thể thiếu phụ phí; cần kiểm tra tổng chi phí thay vì chỉ giá thuê.
