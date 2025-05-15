# Onepiece Adventure

## Giới thiệu
Onepiece Adventure là trò chơi platformer 2D chạy trên Java (Java 2D API) với phong cách pixel art. Trò chơi hỗ trợ 1 hoặc 2 người chơi, trong đó người chơi điều khiển hai nhân vật Luffy và Zoro (vẽ lại theo phong cách pixel art riêng). Game có tổng cộng 5 màn chơi với độ khó tăng dần, từ những màn cơ bản đến những màn thử thách. Các NPC (kẻ địch, các đối tượng tương tác) và cơ chế nhảy, va chạm, AI trong game được kế thừa và điều chỉnh từ mã nguồn PlatformerTutorial gốc của KaarinGaming. Mục tiêu là vượt qua các chướng ngại vật, đánh bại kẻ địch và hoàn thành cấp độ.

## Tính năng
- **Chơi đơn hoặc đôi:** Hỗ trợ chế độ chơi đơn và đôi cùng chia sẻ màn hình (sojin).  
- **Nhân vật pixel art:** Luffy và Zoro được vẽ lại theo phong cách pixel art thủ công, mang hơi hướng anime (One Piece) nhưng vẫn phù hợp lối chơi retro.  
- **Năm màn chơi:** Game có 5 cấp độ với độ khó tăng dần, mỗi màn có thiết kế khác nhau (hòn đảo nhiệt đới, thành phố đổ nát, rừng rậm, v.v.).  
- **Cơ chế inherited:** Từ game gốc, giữ lại cơ chế nhảy, va chạm với địa hình, AI đơn giản của kẻ địch, đồng thời thêm thắt một số yếu tố tùy chỉnh cho phù hợp với chủ đề.  
- **Đồ họa và âm thanh:** Sử dụng ảnh nền và âm thanh phù hợp (ví dụ tiếng bước chân, nhạc nền cảnh hành động) với định dạng trong thư mục `res/`.  

## Điều khiển
- **Người chơi 1:** Sử dụng phím `A` (trái), `D` (phải) để di chuyển, phím `W` để nhảy.  
- **Người chơi 2:** Sử dụng phím `←` (trái), `→` (phải) để di chuyển, phím `↑` để nhảy.  
- **Điều khiển chung:** Phím `Esc` tạm dừng hoặc thoát game, phím `P` (nếu có) để tạm dừng (nếu được cài).  

## Cách cài đặt
1. **Cài đặt Java:** Đảm bảo đã cài JDK (Java Development Kit) phiên bản tương thích (ví dụ JDK 11 trở lên) và thiết lập biến môi trường `JAVA_HOME`.  
2. **Tải mã nguồn:** Clone hoặc tải về thư mục dự án từ kho chứa (ví dụ GitHub).  
3. **Biên dịch và chạy:** Sử dụng IDE (Eclipse/IntelliJ) hoặc dòng lệnh `javac` để biên dịch mã nguồn trong thư mục `src/`. Sau khi biên dịch, chạy chương trình chính (ví dụ `Main.java`) bằng lệnh `java`. Nếu có file `.jar`, chạy trực tiếp bằng `java -jar`.  
4. **Thư viện (nếu cần):** Nếu dự án sử dụng thư viện bên ngoài (khá hiếm cho Java 2D thuần), hãy đảm bảo thêm vào classpath.  

## Cấu trúc thư mục
- `src/` – Thư mục chứa mã nguồn Java (các lớp game, luồng game, xử lý va chạm, v.v.).  
- `res/` – Thư mục tài nguyên:
  - `res/images/` – Hình ảnh (pixel art nhân vật Luffy, Zoro, NPC, tileset nền, v.v.).  
  - `res/levels/` – Dữ liệu các màn chơi (ví dụ file JSON hoặc ảnh chứa dữ liệu level).  
  - `res/sound/` – Âm thanh và nhạc nền (nếu có).  
- `lib/` – Thư viện bên ngoài (nếu sử dụng, ví dụ thư viện xử lý âm thanh).  
- `README.md` – Tệp hướng dẫn này.  

## Hình ảnh minh họa (giả lập)
:contentReference[oaicite:2]{index=2}Trong Zoro & Luffy Platformer, bối cảnh có thể là các hòn đảo ngoài khơi trên biển mang đậm không khí phiêu lưu (tương tự vùng biển trong One Piece). Các cảnh hoàng hôn, đại dương, cây cối nhiệt đới… có thể được mô phỏng để tăng tính hấp dẫn.

:contentReference[oaicite:3]{index=3}Thiết kế màn chơi là các nền tảng lơ lửng, đường đi dốc nối các đảo với nhau, cùng với lâu đài hoặc tháp pháo làm phông nền. Hình ảnh ví dụ trên minh họa một phần bản đồ điển hình của game platformer: các khối đá ghép lại tạo bệ, cùng cầu thang và trụ đèn phong cách fantasy.

:contentReference[oaicite:4]{index=4}Tất cả đồ họa nhân vật và các đối tượng (NPC, cửa hàng, biển báo, đồ vật) được vẽ lại theo phong cách pixel. Hình minh họa là một góc nhỏ (cửa hàng nhỏ) vẽ theo pixel art, tương tự như phong cách đồ họa trong game. Luffy, Zoro và NPC khác cũng sẽ được thể hiện với cùng phong cách này để tạo sự đồng nhất.


## Tài liệu tham khảo
**PlatformerTutorial** - KaarinGaming
Pixel Frog
Java Object Oriented Programming Series - Caleb Curry
