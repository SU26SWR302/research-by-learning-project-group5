# TOURMATE - SWD392 Group 5 - Sum26

TourMate là nền tảng du lịch thông minh kết hợp trải nghiệm ảo trước chuyến đi dưới dạng game, quản lý tour thực tế theo thời gian thực, và kết nối P2P không cần internet. Mục tiêu là xóa bỏ ranh giới giữa chuẩn bị — trải nghiệm — và kỷ niệm trong một hành trình du lịch hoàn chỉnh.

## Group 5 - Team Members

- Lê Đức Sự
- Lê Viết Mạnh
- Phạm Thị Vân Thanh
- Hoàng Thủy Nguyên
- Huỳnh Tấn Vinh

## Jira Link

Jira project link: https://vaanthanh2005.atlassian.net/jira/software/projects/SCRUM/summary?atlOrigin=eyJpIjoiZDg4NjQ3NTNlZWMwNDg2Nzg2MTVhZmMxNjQ2ZjgwYTgiLCJwIjoiaiJ9

## Documentations - RDS

Link RDS documentation:  
https://docs.google.com/document/d/1TkzdZRSMXzru4KWArm73BzWpnXa4SvUaAgt468msgJk/edit?usp=sharing

## Back-end Source Code

Back-end source code:

## Front-end Source Code

Front-end source code:

## Requirements-Based Learning (RBL) Focus

- Nghiên cứu sâu ý tưởng "Xây dựng bản đồ du lịch ảo (build map) tích hợp dữ liệu cá nhân".
- Lý do chọn: Bản đồ tương tác là ngách khả thi và có giá trị thực tế cao, giúp TourMate khác biệt khi trình bày trải nghiệm du lịch theo không gian.
- Hướng nghiên cứu: tập trung vào cách thiết kế, hiển thị và tối ưu hoá bản đồ khu du lịch; kết hợp data vị trí, điểm tham quan, thời tiết và sở thích để tăng tính cá nhân hoá.
- Kết quả kỳ vọng: một giải pháp build map rõ ràng với mô hình đánh giá và đề xuất điểm tham quan dựa trên bản đồ, giúp người dùng thấy ngay nơi phù hợp và tránh chọn sai địa điểm.

## About TourMate

TourMate là nền tảng giúp người dùng trải nghiệm ảo các khu du lịch trước khi quyết định có nên đến hay không. Thay vì chỉ xem ảnh tĩnh hay đọc review, người dùng có thể khám phá bản đồ khu du lịch, xem video POV từng hoạt động, nhận gợi ý cá nhân hóa theo sở thích, thể trạng, thời tiết và ngân sách.
Điểm khác biệt cốt lõi so với các app du lịch hiện tại: TourMate không chỉ cho biết khu đó có gì, mà giúp người dùng biết khu đó có hợp với mình không trước khi đặt vé.

### Mục tiêu

- Giúp người dùng khám phá trực quan khu du lịch bằng bản đồ, video POV và nội dung tương tác.
- Dự đoán mức độ phù hợp của mỗi địa điểm dựa trên sở thích cá nhân, thể trạng, thời tiết và ngân sách.
- Tránh việc chọn sai hành trình bằng cách cung cấp gợi ý du lịch cá nhân hoá trước khi đặt vé.

### Điểm khác biệt chính

- Không chỉ cung cấp thông tin: TourMate có khả năng đánh giá mức độ phù hợp cho từng người dùng.
- Kết nối dữ liệu thực tế: thời tiết, sức khỏe, sở thích và điều kiện di chuyển được dùng làm đầu vào cho hệ thống gợi ý.
- Thắng-thua nhờ trải nghiệm ảo: người dùng có thể xem trước hoạt động dưới dạng video và ảnh 360/POV.

### Các tính năng chính

1. Quiz sở thích
   - Người dùng trả lời chuỗi câu hỏi ngắn: thích mạo hiểm hay thư giãn, đi một mình hay gia đình có trẻ em, ngân sách dự kiến, sức khỏe, thời gian dự định.
   - Hệ thống xếp hạng và ưu tiên hiển thị các khu du lịch phù hợp.

2. Bản đồ khu du lịch
   - Hiển thị bản đồ 2D dạng SVG hoặc ảnh tương tác của từng khu.
   - Người dùng click vào từng điểm để xem ảnh, video và thông tin chi tiết.
   - Nơi có Street View công khai sẽ nhúng Google Maps hoặc Mapillary API; nơi chưa có dùng ảnh tĩnh và video embed.

3. Video POV
   - Mỗi hoạt động có 3-5 video dự phòng từ YouTube, TikTok, Facebook.
   - Hệ thống tự động kiểm tra trạng thái video hàng tuần và chuyển sang nguồn backup khi cần.

4. AI gợi ý thông minh
   - Kết hợp vị trí hiện tại, thời tiết thực tế và dự báo, sức khỏe và thể trạng đã khai báo.
   - Đưa ra đề xuất cụ thể cho hoạt động phù hợp, ví dụ: "Hôm nay Bà Nà Hills có mưa buổi chiều, phù hợp đi Fantasy Park trong nhà hơn là Cầu Vàng ngoài trời."

5. Thanh thể lực
   - Mỗi hoạt động gắn cường độ và thời gian tiêu hao.
   - Hệ thống tính toán số hoạt động phù hợp trong ngày và gợi ý thứ tự trải nghiệm.

6. Giá vé và ưu đãi
   - Nhập dữ liệu ban đầu bằng thủ công, sau đó cập nhật định kỳ.
   - Nút mua vé dẫn thẳng tới trang chính thức, không qua trung gian.

7. Nội quy và an toàn
   - Mỗi hoạt động đính kèm giới hạn chiều cao, cân nặng, độ tuổi và cảnh báo nguy hiểm.
   - Hiển thị thông tin an toàn trước khi người dùng xem video.

8. Danh sách vật dụng thông minh
   - Tổng hợp dựa trên hoạt động người dùng chọn và dự báo thời tiết ngày đi.
   - Mỗi vật dụng đi kèm lý do cụ thể theo hoạt động hoặc điều kiện thời tiết.

### Chiến lược nội dung theo giai đoạn

- Lớp 1: Dùng dữ liệu công khai, Google Maps Street View API và Mapillary API, ảnh Photosphere, video embed từ nguồn miễn phí.
- Lớp 2: Hợp tác với vlogger và khu du lịch để lấy nội dung chất lượng cao, tích hợp YouTube Data API và TikTok API.
- Lớp 3: Phát triển marketplace video, cho phép upload nội dung trả phí, và mở rộng virtual tour 3D.

### Chiến lược Street View

Không tự xây Street View hoàn chỉnh vì quá tốn kém và không thể cạnh tranh về chất lượng với Google. Thay vào đó chia thành 3 trường hợp.

- Trường hợp 1: Nơi có Street View công khai, nhúng Google Maps Embed API hoặc Mapillary API.
- Trường hợp 2: Nơi có Photosphere do cộng đồng đóng góp, dùng làm điểm 360 tĩnh.
- Trường hợp 3: Nơi thiếu dữ liệu, dùng bản đồ 2D + ảnh tĩnh + video làm fallback.
- Navigation kiểu GeoGuessr chỉ thực hiện khi đã có partnership và đủ ảnh 360 liên tục.
