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

This project focuses on Requirements-Based Learning (RBL) methodologies.

## Research Papers References

## About TourMate
Mục tiêu cốt lõi Giúp người dùng trải nghiệm ảo các hoạt động bên trong khu du lịch trước khi quyết định có nên đến hay không, đồng thời chuẩn bị đầy đủ thông tin thực tế và cá nhân hóa gợi ý theo từng người.
### Target Users

- **Khách du lịch (Tourist)**: Người tham gia tour hoặc tự đi, muốn khám phá địa điểm đầy đủ, không bị lạc, và hiểu sâu hơn về nơi mình đến.
- **Hướng dẫn viên chuyên nghiệp (Guide)**: Người tổ chức và dẫn tour, cần quản lý đoàn, theo dõi vị trí thành viên, và đảm bảo không ai bị bỏ lại.
- **Khách tự hướng dẫn (Self-Guide)**: Người muốn tự khám phá mà không cần guide, dựa hoàn toàn vào kiến thức và công cụ có sẵn trong app.

### 4 Module chính



#### Cơ chế chính 

Trải nghiệm ảo Người dùng di chuyển trong khu → đến gần điểm nổi bật → bấm "Tham gia" → xem video trải nghiệm góc nhìn thứ nhất (POV) của hoạt động đó → bấm Thích hoặc Bỏ qua → hệ thống tổng hợp sở thích và gợi ý khu phù hợp nhất.
________________________________________
#### Cơ chế Quiz gợi ý địa điểm 

Trước khi vào trải nghiệm ảo, người dùng trả lời một chuỗi câu hỏi ngắn: thích mạo hiểm hay thư giãn, đi một mình hay gia đình có trẻ em, ngân sách dự kiến bao nhiêu, sức khỏe thế nào, muốn đi bao lâu. Dựa trên kết quả quiz, hệ thống xếp hạng các khu du lịch phù hợp và ưu tiên hiển thị những khu đó lên đầu.
________________________________________
#### Cơ chế AI gợi ý thông minh 
AI phân tích đồng thời ba yếu tố: vị trí hiện tại của người dùng, thời tiết thực tế và dự báo tại khu du lịch trong ngày dự định đi, tình trạng sức khỏe và thể trạng đã khai báo. Từ đó đưa ra gợi ý cụ thể như "Hôm nay Bà Nà Hills có mưa buổi chiều, phù hợp đi Fantasy Park trong nhà hơn là Cầu Vàng ngoài trời" hoặc "Cách bạn 45 phút, phù hợp đi về trong ngày không cần nghỉ đêm."
________________________________________
#### Cơ chế dữ liệu thực tế


Thanh thể lực: mỗi hoạt động tiêu tốn thể lực dựa trên cường độ và thời gian. Người dùng nhập thể trạng, có trẻ em hoặc người lớn tuổi không → hệ thống tính được chơi bao nhiêu trò trong một ngày và gợi ý thứ tự hợp lý.
Giá vé và ưu đãi: tự động cào giá từ trang chính chủ của từng khu theo lịch định kỳ để luôn hiển thị giá mới nhất. Khi người dùng quyết định đi, nút "Mua vé" trỏ thẳng tới trang bán vé chính thức, không qua trung gian.
Lọc theo giá và sở thích: lọc theo khoảng giá vé, loại hình (thiên nhiên, giải trí, văn hóa, nghỉ dưỡng), khoảng cách từ vị trí hiện tại, phù hợp với đối tượng (gia đình, cặp đôi, nhóm bạn, solo).
Nội quy và lưu ý an toàn: mỗi hoạt động đính kèm giới hạn chiều cao, cân nặng, độ tuổi, cảnh báo nguy hiểm. Hiển thị trước khi xem video.
Lịch sử và di sản: với điểm văn hóa như nhà cổ, chùa, làng nghề — cung cấp nội dung ngắn về lịch sử, ý nghĩa, điều thú vị ít người biết.
Vật dụng cần mang — kết hợp hoạt động và thời tiết: danh sách vật dụng được tổng hợp từ hai nguồn đồng thời. Nguồn một là các hoạt động người dùng đã chọn Thích (ví dụ tàu lượn → giày buộc chắc, không đội mũ rộng vành). Nguồn hai là thời tiết thực tế ngày dự định đi (ví dụ trời mưa → thêm áo mưa, giày chống trơn; trời nắng nóng → thêm kem chống nắng, nước uống nhiều hơn; trời lạnh trên núi → thêm áo khoác dày, găng tay). Hai nguồn kết hợp lại mới ra danh sách cuối cùng, mỗi vật dụng đều có lý do cụ thể gắn với hoạt động hoặc thời tiết tương ứng.
Thời tiết và thời điểm: tích hợp dữ liệu thời tiết theo mùa, cảnh báo mùa mưa hoặc đông khách, gợi ý khung giờ tốt nhất trong ngày cho từng điểm.

