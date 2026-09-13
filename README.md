<<<<<<< HEAD
# 🚀 MiaoZi XiaoYao Engine (MiaoZi JS)

**MiaoZi XiaoYao Engine** là một Game Engine đa nền tảng, bứt phá giới hạn, được phát triển độc quyền bởi Kỹ sư **Nguyễn Hiệp** (XiaoYao) (SN 1999 - Admin **MiaoZiGame** / Miêu Tử Game /Mèo Con Game). 

Engine được tối ưu hóa toàn diện từ mã nguồn Front-end React đến vỏ bọc Electron. Dự án hướng tới một triết lý phát triển game **Thuần Offline độc lập (Godot-style)**, bảo mật chống hack cực hạn, nhưng sở hữu **Hạ tầng kết nối mạng Multiplayer và Trí tuệ nhân tạo (AI 3D) tự chủ siêu cấp**.

---

## ✨ Các tính năng nâng cấp cốt lõi (Core Advanced Features)

### 🎨 Đồ Họa Đỉnh Cao & Trí Tuệ Nhân Tạo (AI & 3D Graphics)
* **🤖 AI 3D Game Generation:** Tích hợp bộ xử lý mô hình trí tuệ nhân tạo ngay trong nhân Engine, hỗ trợ tự động tính toán, tối ưu lịch trình và bẻ góc ghim tâm thời gian thực cho các thực thể AI 3D thông minh.
* **⚡ Siêu tối ưu hóa đồ họa (Graphics Upscale):** Thuật toán gộp Mesh tĩnh nội địa, tối ưu hóa bộ đệm nhị phân `Float32Array` giao tiếp thẳng với VRAM/GPU, giúp giữ vững mốc 60 FPS cực mượt, không tụt hiệu năng, giảm sinh nhiệt và tiết kiệm pin phần cứng tối đa.

### 🌐 Hạ Tầng Mạng Multiplayer Tự Chủ (Networking & Servers)
* **🛡️ Dedicated Nakama Server Support:** Tích hợp sẵn kiến trúc kết nối đến hệ thống Backend server Nakama riêng biệt. Cho phép nhà phát triển tự chủ quản lý dữ liệu tài khoản, bảng xếp hạng (Leaderboard), bang hội (Guild) và hệ thống kinh tế MMORPG toàn cục.
* **🔗 Peer JS P2P Dedicated Network:** Lõi WebRTC ngang hàng qua server Peer JS riêng biệt, tối ưu hóa độ trễ (Ping) về mốc chớp mắt, chống mất gói tin (Packet loss) và tự động Reconnect thông minh cho các trận đấu PvP trực tiếp.
* **⚡ Kỹ thuật mạng nâng cao:** Mã hóa chuỗi nén dữ liệu siêu phẳng, truyền tải thông tin thực thể mượt mà xuyên đa chiều không gian mạng.

### 📜 Lập Trình & Bảo Mật Thần Cấp (Scripting & Ultimate Security)
* **💻 Ngôn ngữ kịch bản MiaoZi JS:** Ngôn ngữ lập trình được Nguyễn Hiệp (XiaoYao) thiết kế riêng cho Engine. Cú pháp ngắn gọn, sạch sẽ, giải mã Method Chaining tốc độ cực hạn, tích hợp sẵn các siêu phương thức như `.sp()`, `.spadd()`, xử lý ma trận và lịch pháp tử vi hoàng kim vạn năm.
* **🛡️ Bảo mật chống Cheat/Hack:** Lớp tường lửa lõi mã hóa động ngăn chặn 100% các hành vi can thiệp VRAM, hack bất tử, lận đồ hoặc chỉnh sửa bộ nhớ client từ các công cụ gian lận ngoài sảnh.

### 📐 Giao Diện Khách Hàng (UI/UX Customization)
* **🎨 Sáng tạo UI không giới hạn qua HTML & CSS:** Toàn bộ giao diện người dùng, thanh công cụ, bảng đa lựa chọn Cyberpunk được dựng trực tiếp bằng HTML5 và CSS3 layout (vw/vh, Flexbox, Grid), làm UI game dễ dàng và đẹp mắt như thiết kế website chuyên nghiệp.
* **💾 Lưu trữ cục bộ mặc định (Godot-style):** Ép hệ thống ưu tiên lưu dự án trực tiếp vào ổ đĩa máy tính (`Local File`) thay vì đám mây, bảo vệ quyền riêng tư và tài sản trí tuệ tuyệt đối cho lập trình viên.

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
=======
![GDevelop logo](https://raw.githubusercontent.com/4ian/GDevelop/master/newIDE/GDevelop%20banner.png "GDevelop logo")

GDevelop is a **full-featured, no-code, open-source** game development software. You can build **2D, 3D and multiplayer games** for mobile (iOS, Android), desktop and the web. GDevelop is designed to be fast and incredibly intuitive: make games using an easy-to-understand yet powerful event-based system and modular behaviors. Create with AI that assists or builds alongside you.

![The GDevelop editor when editing a game level](https://raw.githubusercontent.com/4ian/GDevelop/master/newIDE/GDevelop%20screenshot.png "The GDevelop editor when editing a 3D game level")

![The GDevelop editor when editing a game level](./newIDE/GDevelop%202D%20screenshot.png "The GDevelop editor when editing a 2D game level")

## Getting started

| ❔ I want to...                                   | 🚀 What to do                                                                                                                                                     |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 Use GDevelop to make games                     | Go to [GDevelop homepage](https://gdevelop.io) to download the app!                                                                                               |
| ⚙️ Create/improve an extension                    | Read about [creating an extension](https://wiki.gdevelop.io/gdevelop5/extensions/create), with no-code or code.                                                   |
| 🧑‍💻 Contribute to the editor or game engine        | Follow this [README](newIDE/README.md).                                                                                                                           |
| 👾 Create or sell a game template                 | Submit a [free example or a paid template on the Asset Store](https://wiki.gdevelop.io/gdevelop5/community/guide-for-submitting-an-example/).                     |
| 🎨 Share or sell an asset pack                    | Submit a [free or paid asset pack on the Asset Store](https://wiki.gdevelop.io/gdevelop5/community/sell-asset-pack-store).                                        |
| 🌐 Help translate GDevelop                        | Go on the [GDevelop project on Crowdin](https://crowdin.com/project/gdevelop) or translate [in-app tutorials](https://github.com/GDevelopApp/GDevelop-tutorials). |
| 👥 Get online game services or commercial support | See offers for [professionals, teams or individual creators](https://gdevelop.io/pricing).                                                                        |

> Are you interested in contributing to GDevelop for the first time? Take a look at the list of **[good first issues](https://github.com/4ian/GDevelop/issues?q=is%3Aissue+is%3Aopen+label%3A%22%F0%9F%91%8Cgood+first+issue%22)**, **[good first contributions](https://github.com/4ian/GDevelop/discussions/categories/good-first-contribution)** or the **["🏐 not too hard" cards](https://trello.com/b/qf0lM7k8/gdevelop-roadmap?menu=filter&filter=label:Not%20too%20hard%20%E2%9A%BD%EF%B8%8F)** on the Roadmap.

## Games made with GDevelop

- Find GDevelop games on [gd.games](https://gd.games), the gaming platform for games powered by GDevelop.
- See the [showcase of games](https://gdevelop.io/games) created with GDevelop and published on Steam, iOS (App Store), Android (Google Play), Itch.io, Newgrounds, CrazyGames, Poki...

[![Some games made with GDevelop](https://raw.githubusercontent.com/4ian/GDevelop/master/newIDE/GDevelop%20games.png "Some games made with GDevelop")](https://gdevelop.io/games)

## Technical architecture

GDevelop is composed of an **editor**, a **game engine**, an **ecosystem** of extensions as well as **online services** and commercial support.

| Directory     | ℹ️ Description                                                                                                                                                                                                                                                                                           |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Core`        | Core classes, describing the structure of a game and tools to implement the IDE and work with GDevelop games.                                                                                                                                                                                            |
| `GDJS`        | The game engine, written in TypeScript, using PixiJS and Three.js for 2D and 3D rendering (WebGL), powering all GDevelop games.                                                                                                                                                                          |
| `GDevelop.js` | Bindings of `Core`, `GDJS` and `Extensions` to JavaScript (with WebAssembly), used by the IDE.                                                                                                                                                                                                           |
| `newIDE`      | The game editor, written in JavaScript with React, Electron, PixiJS and Three.js.                                                                                                                                                                                                                        |
| `Extensions`  | Built-in extensions for the game engine, providing objects, behaviors and new features. For example, this includes the physics engines running in WebAssembly (Box2D or Jolt Physics for 3D). All the [official and experimental extensions are on this repository](https://github.com/GDevelopApp/GDevelop-extensions). [Community extensions are available here](https://github.com/GDevelopApp/GDevelop-community-list). |

To learn more about GDevelop Architecture, read the [architecture overview here](Core/GDevelop-Architecture-Overview.md).

Pre-generated documentation of the game engine is [available here](https://docs.gdevelop.io).

Status of the tests and builds: [![macOS and Linux build status](https://circleci.com/gh/4ian/GDevelop.svg?style=shield)](https://app.circleci.com/pipelines/github/4ian/GDevelop) [![Fast tests status](https://gdevelop.semaphoreci.com/badges/GDevelop/branches/master.svg?style=shields)](https://gdevelop.semaphoreci.com/projects/GDevelop) [![Windows Build status](https://ci.appveyor.com/api/projects/status/84uhtdox47xp422x/branch/master?svg=true)](https://ci.appveyor.com/project/4ian/gdevelop/branch/master) [![https://good-labs.github.io/greater-good-affirmation/assets/images/badge.svg](https://good-labs.github.io/greater-good-affirmation/assets/images/badge.svg)](https://good-labs.github.io/greater-good-affirmation)

## Links

### Community

- [GDevelop forums](https://forum.gdevelop.io) and [Discord chat](https://discord.gg/gdevelop).
- [GDevelop homepage](https://gdevelop.io).
- [GDevelop wiki (documentation)](https://wiki.gdevelop.io/gdevelop5/start).
- Help translate GDevelop in your language: [GDevelop project on Crowdin](https://crowdin.com/project/gdevelop).
- Open-source [extensions (official or experimental)](https://github.com/GDevelopApp/GDevelop-extensions), [community extensions](https://github.com/GDevelopApp/GDevelop-community-list), [examples](https://github.com/GDevelopApp/GDevelop-examples), [tutorials](https://github.com/GDevelopApp/GDevelop-tutorials) are on GitHub.

### Development Roadmap

- [GDevelop Roadmap on Trello.com](https://trello.com/b/qf0lM7k8/gdevelop-roadmap), for a global view of the features that could be added. Please vote and comment here for new features/requests.
- [GitHub issue page](https://github.com/4ian/GDevelop/issues), for technical issues and bugs.
- [Github discussions](https://github.com/4ian/GDevelop/discussions) to talk about new features and ideas.

## License

- The Core library, the native and HTML5 game engines, the IDE, and all extensions (respectively `Core`, `GDJS`, `newIDE` and `Extensions` folders) are under the **MIT license**.
- The name, GDevelop, and its logo are the exclusive property of Florian Rival.

Games exported with GDevelop are based on the GDevelop game engine (see `Core` and `GDJS` folders): this engine is distributed under the MIT license so that you can **distribute, sell or do anything** with the games you created with GDevelop. In particular, you are not forced to make your game open-source.

[node.js]: https://nodejs.org

## Star History

Help us spread the word about GDevelop by starring the repository on GitHub!

[![Star History Chart](https://api.star-history.com/svg?repos=4ian/gdevelop&type=Date)](https://star-history.com/#4ian/gdevelop&Date)
>>>>>>> 03dae4c (Khoi tao loi MiaoZi XiaoYao Engine)
