
# MiaoZi XiaoYao Engine (MiaoZi JS)

**MiaoZi XiaoYao Engine** là một Game Engine đa nền tảng, bứt phá giới hạn, được phát triển độc quyền bởi Kỹ sư **Nguyễn Hiệp** (XiaoYao) (SN 1999 - Admin **MiaoZiGame** / Miêu Tử Game /Mèo Con Game). 

Engine được tối ưu hóa toàn diện từ mã nguồn Front-end React đến vỏ bọc Electron. Dự án hướng tới một triết lý phát triển game **Thuần Offline độc lập (Godot-style)**, bảo mật chống hack cực hạn, nhưng sở hữu **Hạ tầng kết nối mạng Multiplayer và Trí tuệ nhân tạo (AI 3D) tự chủ siêu cấp**.

---

## ✨ Các tính năng nâng cấp cốt lõi (Core Advanced Features)

### ✨  Đồ Họa Đỉnh Cao & Trí Tuệ Nhân Tạo (AI & 3D Graphics)

### ✨ AI 3D Game Generation:** Tích hợp bộ xử lý mô hình trí tuệ nhân tạo ngay trong nhân Engine, hỗ trợ tự động tính toán, tối ưu lịch trình và bẻ góc ghim tâm thời gian thực cho các thực thể AI 3D thông minh.

### Siêu tối ưu hóa đồ họa (Graphics Upscale):** Thuật toán gộp Mesh tĩnh nội địa, tối ưu hóa bộ đệm nhị phân `Float32Array` giao tiếp thẳng với VRAM/GPU, giúp giữ vững mốc 60 FPS cực mượt, không tụt hiệu năng, giảm sinh nhiệt và tiết kiệm pin phần cứng tối đa.

### Hạ Tầng Mạng Multiplayer Tự Chủ (Networking & Servers)

### Dedicated Nakama Server Support:** Tích hợp sẵn kiến trúc kết nối đến hệ thống Backend server Nakama riêng biệt. Cho phép nhà phát triển tự chủ quản lý dữ liệu tài khoản, bảng xếp hạng (Leaderboard), bang hội (Guild) và hệ thống kinh tế MMORPG toàn cục.

### Peer JS P2P Dedicated Network:** Lõi WebRTC ngang hàng qua server Peer JS riêng biệt, tối ưu hóa độ trễ (Ping) về mốc chớp mắt, chống mất gói tin (Packet loss) và tự động Reconnect thông minh cho các trận đấu PvP trực tiếp.

### Kỹ thuật mạng nâng cao:** Mã hóa chuỗi nén dữ liệu siêu phẳng, truyền tải thông tin thực thể mượt mà xuyên đa chiều không gian mạng.

### 📜 Lập Trình & Bảo Mật Thần Cấp (Scripting & Ultimate Security)

* **💻 Ngôn ngữ kịch bản MiaoZi JS:** Ngôn ngữ lập trình được Nguyễn Hiệp (XiaoYao) thiết kế riêng cho Engine. Cú pháp ngắn gọn, sạch sẽ, giải mã Method Chaining tốc độ cực hạn, tích hợp sẵn các siêu phương thức như `.sp()`, `.spadd()`, xử lý ma trận và lịch pháp tử vi hoàng kim vạn năm.
* 
### Bảo mật chống Cheat/Hack:** Lớp tường lửa lõi mã hóa động ngăn chặn 100% các hành vi can thiệp VRAM, hack bất tử, lận đồ hoặc chỉnh sửa bộ nhớ client từ các công cụ gian lận ngoài sảnh.

### Giao Diện Khách Hàng (UI/UX Customization)

### Sáng tạo UI không giới hạn qua HTML & CSS:** Toàn bộ giao diện người dùng, thanh công cụ, bảng đa lựa chọn Cyberpunk được dựng trực tiếp bằng HTML5 và CSS3 layout (vw/vh, Flexbox, Grid), làm UI game dễ dàng và đẹp mắt như thiết kế website chuyên nghiệp.

### Lưu trữ cục bộ mặc định (Godot-style):** Ép hệ thống ưu tiên lưu dự án trực tiếp vào ổ đĩa máy tính (`Local File`) thay vì đám mây, bảo vệ quyền riêng tư và tài sản trí tuệ tuyệt đối cho lập trình viên.

---

## 🛠️ Hướng dẫn tự Đóng gói Engine (Development Setup)

### 1. Yêu cầu hệ thống (Prerequisites)
* Cài đặt môi trường [Node.js](https://nodejs.org) (Khuyến nghị bản LTS mới nhất).
* Cài đặt công cụ [Git](https://git-scm.com).

### 2. Cài đặt các thư viện phụ thuộc
Mở dòng lệnh tại thư mục dự án và khởi chạy:
```bash
cd newIDE/app
npm install

cd ../electron-app
npm install
```

### 3. Kích nổ tiến trình Đóng gói thành phẩm (.exe)
Nhấp đúp chuột vào tệp tin chạy tự động ở thư mục gốc:
```cmd
AutoBuild.bat
```
*Tệp lệnh `.bat` đã được Nguyễn Hiệp cấu hình nới rộng RAM phần cứng lên 8GB (`--max-old-space-size=8192`) để biên dịch tổng lực Front-end và tự động nhúng mã token bảo mật an toàn.*

Thành phẩm sau khi hoàn tất sẽ xuất hiện trong thư mục `newIDE/electron-app/dist/` dưới dạng bộ cài độc lập.

---

## 🤝 Bản Quyền và Phát Triển (License & Contributing)

* **Nhà sáng tạo ngôn ngữ & Kỹ sư thiết kế:** Nguyễn Hiệp (SN 1999 - ADMIN MIAOZIGAME).
* **Bản quyền độc quyền:** Được khởi tạo và bảo hộ từ ngày 25 tháng 8 năm 2026.
* **Giấy phép:** Tuân thủ theo các điều khoản mã nguồn mở gốc tự do (MIT / GPL v3). Bạn hoàn toàn có thể sử dụng Engine để thương mại hóa các dự án game độc quyền của riêng mình.

---

## ☕ Ủng hộ nhà phát triển (Support Me)

Nếu bạn yêu thích phiên bản Engine tinh gọn và mạnh mẽ này, bạn có thể mời mình một ly cà phê để tiếp thêm động lực nâng cấp các thuật toán lượng tử tiếp theo tại:
👉 **[Buy Me A Coffee của tôi](https://buymeacoffee.com/miao_zi_xiao_yao)**
