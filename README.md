# JAEN - SWD392 Group 5 - Sum26

JAEN là nền tảng học ngôn ngữ trực tuyến thông minh (Smart Language Learning Platform), hoạt động theo mô hình mở cho phép kết nối giữa người học và người sáng tạo nội dung. Hệ thống không chỉ cung cấp các bài học video tĩnh mà còn tích hợp các module tương tác đa dạng (Flashcards, Quizzes, Reading, Listening) , các bài kiểm tra nói/viết đánh giá tự động bằng AI Assessment cùng hệ thống quản lý tiến độ và từ điển cá nhân hóa.

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
- Nghiên cứu sâu ý tưởng: "Xây dựng hệ thống tự động đánh giá và chấm điểm năng lực ngôn ngữ (Nói và Viết) tích hợp AI Assessment"
- Lý do chọn: Việc chấm điểm kỹ năng Nói (Speaking) và Viết (Writing) theo cách truyền thống tốn rất nhiều thời gian và chi phí. Việc ứng dụng AI giúp tạo ra ngách đi đột phá cho JAEN so với các app học tập thông thường, cung cấp phản hồi tức thì cho người học.
- Hướng nghiên cứu: Tập trung vào tối ưu hóa Prompt, xử lý bất đồng bộ kết quả trả về từ mô hình AI, cấu hình hạn mức sử dụng (Quota) cho mỗi tài khoản để tối ưu chi phí hệ thống
- Kết quả kỳ vọng: Đưa ra giải pháp kiến trúc tích hợp AI có khả năng chấm điểm, giải thích chi tiết lỗi sai và phân tích ngữ pháp trong vòng dưới 5 phút, đảm bảo độ ổn định cao.

## About TourMate

JAEN là nền tảng giúp người dùng tiếp cận và học tập các khóa học ngôn ngữ trực tuyến thông qua kho học liệu đa dạng. Thay vì chỉ học lý thuyết tĩnh, người dùng có thể làm bài tập trắc nghiệm, luyện ghi nhớ qua thẻ từ vựng và tham gia các bài test năng lực toàn diện. 
Điểm khác biệt cốt lõi so với các app học ngôn ngữ hiện tại: JAEN không chỉ cung cấp tài liệu học, mà còn tích hợp Trí tuệ nhân tạo (AI) chấm điểm chi tiết bài Nói và bài Viết như một trợ lý cá nhân thực thụ trước khi người học tham dự các kỳ thi chứng chỉ

### Mục tiêu

- Giúp người dùng khám phá trực quan kho khóa học bằng bộ lọc thông minh, bài giảng video và tài liệu tương tác
- Đánh giá chi tiết mức độ chính xác của kỹ năng Nói/Viết dựa trên công nghệ chấm điểm AI thông minh.
- Tối ưu hóa ngân sách và lộ trình học cá nhân hóa bằng cách cho phép xem trước thông tin khóa học và học thử tài liệu miễn phí trước khi quyết định nâng cấp.

### Điểm khác biệt chính

- Không chỉ cung cấp thông tin: JAEN có khả năng tự động chấm điểm và đưa ra giải thích chi tiết cho từng câu hỏi bằng AI.
- Kết nối dữ liệu thực tế: Trạng thái tiến độ học tập, lịch sử lưu từ vựng và kết quả quiz được sử dụng làm đầu vào để tối ưu hóa lộ trình cá nhân.
- Trải nghiệm tương tác đa chiều: Người học có thể ôn tập từ vựng bằng bộ Flashcard sinh động và theo dõi video bài giảng tích hợp mượt mà.

### Các tính năng chính

1. Bộ lọc & Tìm kiếm Khóa học (Search & Filter)
   - Người dùng tìm kiếm theo từ khóa, danh mục khóa học hoặc phân loại theo thẻ: Miễn phí (Free), Trả phí (Paid), Phổ biến, hay Mới nhất.
   - Hệ thống xếp hạng và hiển thị ưu tiên các khóa học được đánh giá cao từ cộng đồng.

2. Quản lý Tiến độ Học tập (Progress Tracking)
   - Hiển thị biểu đồ tiến trình dưới dạng tỷ lệ % hoàn thành bài học trực quan.
   - Người dùng click vào từng bài học để xem trạng thái hoàn thành các module quiz hoặc video bài giảng liên quan.

3. Video bài giảng (Embedded Video Lectures)
   - Mỗi bài học tích hợp video bài giảng được Creator lưu trữ trên YouTube dưới chế độ không công khai (Unlisted) để bảo mật.
   - Hệ thống nhúng trình phát nội dung trực tuyến ổn định nhờ API kết nối bên ngoài.
     
4. AI chấm điểm thông minh (AI Assessment)
   - Kết hợp dữ liệu đầu vào là file ghi âm bài Nói (Speaking) hoặc đoạn văn bài Viết (Writing) do Learner tải lên.
   - Đưa ra đề xuất sửa lỗi cụ thể trong vòng dưới 5 phút, ví dụ: "Phát âm từ này chưa chuẩn trọng âm" hoặc "Cấu trúc câu này lỗi ngữ pháp, nên sửa thành...".

5. Từ điển cá nhân (Personal Dictionary)
   - Mỗi từ vựng được tra cứu khi bôi đen trực tiếp trên tài liệu PDF có thể lưu lại vào bộ nhớ riêng.
   - Hệ thống tự động đồng bộ và gợi ý ôn tập lại từ mới thông qua các bài tập hàng ngày.
     
6. Hệ thống Thanh toán Bảo mật (Secure Payments)
   - Tích hợp cổng thanh toán trực tiếp qua PayPal và VNPAY, đảm bảo giao dịch nhanh chóng và an toàn.
   - Áp dụng quy tắc giá trị thanh toán tối thiểu từ 75,000 VND.
     
7. Kiểm duyệt & Báo cáo Vi phạm (Moderation & Report)
   - Mỗi khóa học hoặc nội dung đính kèm đều có nút Báo cáo vi phạm (Report) dành cho người học khi phát hiện bản quyền sai lệch.
   - Tự động ẩn nội dung hoặc cảnh báo an toàn cho Admin xử lý khi vượt quá ngưỡng quy định.

8. Bộ công cụ Tạo bài tập tương tác (Course Creation Modules)
   - Hỗ trợ Creator tạo học liệu phong phú dựa trên 10 loại module nội dung khác nhau.
   - Bao gồm: Tạo thẻ ghi nhớ (Flashcard), Trắc nghiệm nhiều lựa chọn (Multiple Choice Quiz), và Điền vào chỗ trống (Gap-Fill).

### Chiến lược nội dung theo giai đoạn

- Lớp 1: Dùng dữ liệu bài giảng công khai, nhúng link video YouTube Unlisted, cung cấp tài liệu dạng PDF trực tuyến và các bài tập Quiz trắc nghiệm cơ bản.
- Lớp 2: Hợp tác với các Creator có chứng chỉ chuyên môn cao để xuất bản khóa học chất lượng, tích hợp chấm điểm tự động Nói/Viết bằng AI nhằm tăng tính trải nghiệm
- Lớp 3: Phát triển mô hình marketplace khóa học toàn diện, tối ưu hóa doanh thu chia sẻ tự động và mở rộng thêm các bài thi thử mô phỏng kỳ thi thực tế.

### Chiến lược Quản lý Video & Bảo mật Học liệu

Hệ thống không tự xây dựng máy chủ lưu trữ video hoàn chỉnh vì quá tốn kém và ảnh hưởng tốc độ băng thông. Thay vào đó chia thành 3 trường hợp:

- Trường hợp 1: Video bài giảng chính thức, Creator upload lên kênh YouTube cá nhân dưới dạng Unlisted, hệ thống nhúng qua mã ID bảo mật để phát trên nền tảng.
- Trường hợp 2: Tài liệu học tập bằng văn bản, sử dụng định dạng PDF và kết xuất trực tiếp qua trình xem trực tuyến của hệ thống để Learner không cần tải về.
- Trường hợp 3: Các bài tập tương tác và tài liệu bổ trợ, bắt buộc phải đi qua Authorization Middleware và hệ thống quét virus tự động trước khi hiển thị cho người học.

