# TOURMATE - SWD392 Group 5 - Sum26

TourMate là nền tảng du lịch thông minh kết hợp trải nghiệm ảo trước chuyến đi dưới dạng game, quản lý tour thực tế theo thời gian thực, và kết nối P2P không cần internet. Mục tiêu là xóa bỏ ranh giới giữa chuẩn bị — trải nghiệm — và kỷ niệm trong một hành trình du lịch hoàn chỉnh.

## Group 5 - Team Members

- Lê Đức Sự
- Lê Viết Mạnh
- Phạm Thị Vân Thanh
- Trần Thủy Nguyên
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

## Jira Link

Jira project link: https://vaanthanh2005.atlassian.net/jira/software/projects/SCRUM/summary?atlOrigin=eyJpIjoiZDg4NjQ3NTNlZWMwNDg2Nzg2MTVhZmMxNjQ2ZjgwYTgiLCJwIjoiaiJ9

## Research Papers

## About TourMate

Khách du lịch (Tourist) — Người tham gia tour hoặc tự đi, muốn khám phá địa điểm đầy đủ, không bị lạc, và hiểu sâu hơn về nơi mình đến.
Hướng dẫn viên chuyên nghiệp (Guide) — Người tổ chức và dẫn tour, cần quản lý đoàn, theo dõi vị trí thành viên, và đảm bảo không ai bị bỏ lại.
Khách tự hướng dẫn (Self-Guide) — Người muốn tự khám phá mà không cần guide, dựa hoàn toàn vào kiến thức và công cụ có sẵn trong app.

---

4 Module chính

---

Module 1 — Dữ liệu khu du lịch
Đây là nền tảng của toàn bộ hệ thống. App xây dựng và duy trì một cơ sở dữ liệu chi tiết về các khu du lịch, bao gồm:
Danh sách từng địa điểm trong khu: tên, tọa độ GPS, mô tả ngắn, mô tả chi tiết, giờ hoạt động, ảnh thực tế, câu chuyện lịch sử và văn hóa đặc trưng. Bố cục tổng thể của khu: các khu vực, lối đi, điểm tập hợp, lối thoát hiểm. Lộ trình mẫu chia theo thời gian: 2 tiếng, nửa ngày, cả ngày. Nội dung kiến thức dạng bài đọc ngắn tại từng điểm — được viết dễ hiểu, phù hợp cho mọi lứa tuổi.
Dữ liệu được đóng góp từ ba nguồn: admin hệ thống, hướng dẫn viên đã được xác minh, và cộng đồng người dùng (có kiểm duyệt). Nguồn ban đầu có thể kéo từ Google Places API, Wikipedia tiếng Việt, và hợp tác trực tiếp với ban quản lý khu du lịch.

---

Module 2 — Pre-trip Game Experience (Trải nghiệm ảo trước chuyến đi)
Đây là tính năng phân biệt TourMate với mọi app du lịch khác hiện tại.
Cơ chế hoạt động
Khu du lịch được tái hiện dưới dạng thế giới 2D top-down đơn giản — phong cách flat map hoặc pixel art nhẹ, ưu tiên nội dung hơn đồ họa. Khách điều khiển nhân vật di chuyển qua từng địa điểm, dừng lại để tương tác và khám phá.
Khi nhân vật đến một địa điểm, app hiển thị ảnh thực tế, mô tả ngắn, và 1-2 câu hỏi kiến thức nhỏ. Trả lời đúng thì mở khóa huy hiệu "đã biết trước" cho địa điểm đó. Toàn bộ nội dung game được kéo thẳng từ database khu du lịch — không cần tạo nội dung riêng.
Hệ thống trạng thái địa điểm
Mỗi địa điểm có ba trạng thái theo vòng đời trải nghiệm: Chưa khám phá → Đã thấy trong game → Đã đến thật. Khi khách đi tour thực tế và check-in tại chỗ, trạng thái được nâng cấp lên. Điều này tạo ra một vòng lặp cảm xúc rõ ràng: thấy ảo trước, đến thật sau, cảm giác quen thuộc ngay từ bước đầu đặt chân vào khu.
Gợi ý lịch trình thông minh
Sau khi chơi game, app phân tích hành vi: khách dừng lại lâu ở đâu, tương tác nhiều với loại địa điểm nào, bỏ qua loại nào. Từ đó tự động gợi ý lịch trình thực tế phù hợp với sở thích cá nhân.
Chơi cùng nhau trước khi đi
Cả đoàn có thể vào cùng một "phòng game" trước chuyến đi — cùng khám phá ảo, cùng trả lời câu hỏi, tạo không khí hào hứng và gắn kết trước khi gặp nhau ngoài thực tế.

---

Module 3 — Quản lý tour thực tế (Guide Dashboard)
Tạo và quản lý tour
Guide tạo tour mới trong vài bước: chọn khu du lịch, đặt tên tour, chọn lịch trình, tạo mã QR để khách tham gia. Khách quét mã là tự động vào đoàn, không cần thêm bước nào.
Theo dõi đoàn theo thời gian thực
Guide thấy được vị trí của từng thành viên trên bản đồ khu du lịch đã tải sẵn. Trạng thái online/offline của từng người hiển thị rõ ràng. Nếu một thành viên tách khỏi đoàn quá xa hoặc mất kết nối P2P quá lâu, app lập tức cảnh báo guide.
Check-in địa điểm
Khi đoàn đến một điểm, guide hoặc từng khách tự check-in bằng GPS hoặc quét QR đặt tại chỗ. Địa điểm được đánh dấu "đã đến" trong lịch trình, kèm thời gian và ghi chú tùy chọn. Cuối tour, toàn bộ hành trình được lưu lại dưới dạng tổng kết có thể xem lại và chia sẻ.
Chat nội bộ nhóm
Tin nhắn văn bản trong đoàn truyền qua P2P — không cần internet, hoạt động ngay cả ở vùng không có sóng.

---

Module 4 — Kết nối P2P (Không cần WiFi)
Đây là xương sống kỹ thuật giúp TourMate hoạt động được ở những nơi đẹp nhất — hang động, rừng quốc gia, đảo xa, vùng núi cao — đúng những nơi mà sóng điện thoại thường không có.
Cơ chế kết nối
Bluetooth Mesh là phương thức chính. Các thiết bị trong đoàn tự kết nối với nhau tạo thành mạng lưới nhỏ. Dữ liệu vị trí và tin nhắn được truyền từ máy này sang máy kia theo chuỗi — máy ở đầu đoàn vẫn nhận được thông tin từ máy ở cuối đoàn thông qua các máy ở giữa làm cầu nối. Phạm vi thực tế của Bluetooth mỗi thiết bị khoảng 30-50m, nhưng với mesh 10 người dàn trải, tầm phủ thực tế có thể lên đến 200-300m.
WiFi Direct là phương thức bổ sung khi cần phạm vi rộng hơn hoặc truyền dữ liệu lớn hơn như ảnh check-in.
Offline-first
Toàn bộ dữ liệu khu du lịch được tải xuống thiết bị trước khi khởi hành. Mọi thao tác trong hành trình — check-in, chat, vị trí, ghi chú — đều lưu local trước. Khi có mạng trở lại, app tự đồng bộ lên server, không mất bất kỳ dữ liệu nào.
Lưu ý kỹ thuật
Trên Android dùng BLE (Bluetooth Low Energy) hoặc thư viện Bridgefy. Trên iOS dùng MultipeerConnectivity framework vì Apple hạn chế WiFi Direct trực tiếp. Đây là phần phức tạp nhất về kỹ thuật và cần được prototype sớm để đánh giá giới hạn thực tế.

---

Module 5 — Tự trở thành hướng dẫn viên (Self-Guide Mode)
Bất kỳ người dùng nào cũng có thể kích hoạt chế độ này mà không cần đăng ký làm guide chuyên nghiệp.
Khách tự tạo lịch trình cá nhân từ danh sách địa điểm trong khu. App cung cấp toàn bộ kiến thức — lịch sử, văn hóa, mẹo tham quan, câu chuyện thú vị — đủ để tự dẫn mình và người thân đi một cách tự tin. Tự check-in từng nơi, nhận huy hiệu hoàn thành lộ trình. Lịch trình cá nhân sau khi hoàn thành có thể lưu lại và chia sẻ cho người khác dùng lại — dần dần xây dựng một kho lịch trình do cộng đồng đóng góp.

---

Module 6 — Đăng ký Hướng dẫn viên chuyên nghiệp
Guide đăng ký tài khoản, khai báo khu du lịch phụ trách, và được xác minh qua quy trình duyệt của admin hoặc đánh giá từ cộng đồng. Sau khi được duyệt, guide có thể đóng góp nội dung vào database: thêm địa điểm, viết mô tả chi tiết hơn, bổ sung câu chuyện địa phương độc quyền, thêm câu hỏi quiz cho game. Hồ sơ guide hiển thị công khai: kinh nghiệm, ngôn ngữ dẫn tour, đánh giá từ khách đã đi. Khách có thể tìm kiếm và liên hệ guide phù hợp trực tiếp trong app.

---

Vòng đời trải nghiệm hoàn chỉnh
Trước chuyến đi, khách nhận mã tour từ guide, vào chế độ game khám phá ảo khu du lịch tại nhà, cùng cả đoàn chơi chung để tạo không khí, và nhận gợi ý lịch trình cá nhân hóa dựa trên sở thích game.
Ngày khởi hành, mọi người mở app và tự động kết nối P2P với nhau qua Bluetooth — không cần WiFi, không cần thao tác thêm. Toàn bộ dữ liệu khu đã có sẵn offline trong máy.
Trong hành trình, guide theo dõi đoàn trên bản đồ offline, nhận cảnh báo ngay nếu ai tách xa, chat nhóm qua P2P. Mỗi khi đến một địa điểm đã "thấy trong game", khách check-in để nâng cấp trạng thái lên "đã đến thật" — cảm giác hoàn thành rõ rệt.
Kết thúc tour, app tổng kết toàn bộ hành trình: số địa điểm đã đến, điểm kiến thức, huy hiệu, bản đồ hành trình. Khi có mạng, dữ liệu đồng bộ lên cloud. Khách có thể chia sẻ hành trình của mình.

---

Rủi ro và thách thức chính
Kỹ thuật P2P là phần khó nhất — cần prototype sớm để kiểm tra giới hạn thực tế của Bluetooth mesh trên các thiết bị đa dạng. Chất lượng dữ liệu khu du lịch quyết định giá trị của toàn bộ app — cần đầu tư nghiêm túc vào việc thu thập và kiểm duyệt nội dung ngay từ đầu. Game mechanics cần đủ hấp dẫn để khách thực sự chơi trước khi đi, không chỉ là một tính năng thêm vào cho có.
