![MiaoZi XiaoYao Engine banner](https://githubusercontent.com "MiaoZi XiaoYao Engine banner")

# MiaoZi XiaoYao Engine (MiaoZi JS)

**MiaoZi XiaoYao Engine** là một Game Engine đa nền tảng, bứt phá giới hạn, được phát triển và tùy biến sâu bởi Kỹ sư **Nguyễn Hiệp (XiaoYao)** (SN 1999 - Admin **MiaoZiGame** / Miêu Tử Game / Mèo Con Game). 

Engine được tối ưu hóa toàn diện từ mã nguồn Front-end React đến vỏ bọc Electron. Dự án hướng tới một triết lý phát triển game **Thuần Offline độc lập (Godot-style)**, bảo mật chống hack cực hạn, nhưng sở hữu **Hạ tầng kết nối mạng Multiplayer và Trí tuệ nhân tạo (AI 3D) tự chủ siêu cấp**.

---

## ✨ Các tính năng nâng cấp cốt lõi (Core Advanced Features)

### 📊 Đồ Họa Đỉnh Cao & Trí Tuệ Nhân Tạo (AI & 3D Graphics)
* **Siêu tối ưu hóa đa nền tảng:** Cả phần xử lý đồ họa **2D và 3D đều đã được tối ưu hóa hoàn hảo, có thể chạy mượt mà trên bất kỳ máy cấu hình yếu nào với chất lượng đồ họa cao cấp**.
* **AI 3D Game Generation:** Tích hợp bộ xử lý mô hình trí tuệ nhân tạo ngay trong nhân Engine, hỗ trợ tự động tính toán, tối ưu lịch trình và bẻ góc ghim tâm thời gian thực cho các thực thể AI 3D thông minh.
* **Tối ưu hóa phần cứng (Graphics Upscale):** Thuật toán gộp Mesh tĩnh nội địa, tối ưu hóa bộ đệm nhị phân `Float32Array` giao tiếp thẳng với VRAM/GPU, giúp giữ vững mốc 60 FPS cực mượt, không tụt hiệu năng, giảm sinh nhiệt và tiết kiệm pin phần cứng tối đa.

### 🌐 Hạ Tầng Mạng Multiplayer Tự Chủ (Networking & Servers)
* **Dedicated Nakama Server Support:** Tích hợp sẵn kiến trúc kết nối đến hệ thống Backend server Nakama riêng biệt. Cho phép nhà phát triển tự chủ quản lý dữ liệu tài khoản, bảng xếp hạng (Leaderboard), bang hội (Guild) và hệ thống kinh tế MMORPG toàn cục.
* **Peer JS P2P Dedicated Network:** Lõi WebRTC ngang hàng qua server Peer JS riêng biệt, tối ưu hóa độ trễ (Ping) về mốc chớp mắt, chống mất gói tin (Packet loss) và tự động Reconnect thông minh cho các trận đấu PvP trực tiếp.
* **Kỹ thuật mạng nâng cao:** Mã hóa chuỗi nén dữ liệu siêu phẳng, truyền tải thông tin thực thể mượt mà xuyên đa chiều không gian mạng.

### 🔎 Lập Trình & Bảo Mật Thần Cấp (Scripting & Ultimate Security)
* **💻 Ngôn ngữ kịch bản MiaoZi JS:** Ngôn ngữ kịch bản được Nguyễn Hiệp (XiaoYao) thiết kế riêng cho Engine. Cú pháp ngắn gọn, sạch sẽ, giải mã Method Chaining tốc độ cực hạn, tích hợp sẵn các siêu phương thức như `.sp()`, `.spadd()`, xử lý ma trận và lịch pháp tử vi hoàng kim vạn năm.
* **⚠️ Bảo mật chống Cheat/Hack:** Lớp tường lửa lõi mã hóa động ngăn chặn 100% các hành vi can thiệp VRAM, hack bất tử, lận đồ hoặc chỉnh sửa bộ nhớ client từ các công cụ gian lận ngoài sảnh.

### 🗒 Giao Diện Khách Hàng (UI/UX Customization)
* **Sáng tạo UI không giới hạn qua HTML & CSS:** Toàn bộ giao diện người dùng, thanh công cụ, bảng đa lựa chọn Cyberpunk được dựng trực tiếp bằng HTML5 và CSS3 layout (vw/vh, Flexbox, Grid), làm UI game dễ dàng và đẹp mắt như thiết kế website chuyên nghiệp.
* **Lưu trữ cục bộ mặc định (Godot-style):** Ép hệ thống ưu tiên lưu dự án trực tiếp vào ổ đĩa máy tính (`Local File`) thay vì đám mây, bảo vệ quyền riêng tư và tài sản trí tuệ tuyệt đối cho lập trình viên.

---

## 🗒 Technical Architecture

MiaoZi XiaoYao Engine được phân chia thành cấu trúc các thư mục lõi sau để nhà phát triển dễ dàng can thiệp tùy biến:

| Directory | ℹ️ Description |
| --------- | ------------- |
| `Core`    | Lớp lõi xử lý, mô tả cấu trúc của một dự án game và các công cụ làm việc với hệ thống. |
| `GDJS`    | Game engine chính, được tối ưu hóa bằng TypeScript, sử dụng PixiJS và Three.js cho kết xuất đồ họa 2D/3D. |
| `newIDE`  | Trình biên tập trực quan (Editor) của Engine, xây dựng trên nền tảng React và Electron. |

---

## 🛠️ Hướng dẫn tự Đóng gói Engine (Development Setup)

### 1. Yêu cầu hệ thống (Prerequisites)
* Cài đặt môi trường [Node.js](https://nodejs.org) (Khuyến nghị bản LTS mới nhất).
* Cài đặt công cụ [Git](https://git-scm.com).

### 2. Cài đặt các thư viện phụ thuộc
Mở dòng lệnh Terminal tại thư mục dự án và khởi chạy:
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

## ☕ Ủng hộ nhà phát triển

Nếu bạn yêu thích phiên bản Engine tinh gọn và mạnh mẽ này, bạn có thể mời mình một ly cà phê để tiếp thêm động lực nâng cấp các thuật toán lượng tử tiếp theo tại:
👉 **[Buy Me A Coffee của tôi](https://buymeacoffee.com/miao_zi_xiao_yao)**


![MiaoZi XiaoYao Engine banner](https://githubusercontent.com "MiaoZi XiaoYao Engine banner")

# MiaoZi XiaoYao Engine (MiaoZi JS)

**MiaoZi XiaoYao Engine** is a cutting-edge, cross-platform game engine deeply customized and developed by Engineer **Nguyen Hiep (XiaoYao)** (Born in 1999 - Admin of **MiaoZiGame**). 

The engine is comprehensively optimized from the React front-end architecture to the Electron container. The project is driven by a **purely offline and independent workflow (Godot-style)**, featuring ultimate anti-cheat protection, autonomous multiplayer networking infrastructure, and sovereign 3D AI computing capabilities.

---

## ✨ Core Advanced Features

### 📊 Advanced 3D/2D Graphics & Artificial Intelligence
* **Flawless Multi-Platform Optimization:** Both **2D and 3D rendering pipelines are flawlessly optimized, enabling high-end graphical quality to run smoothly on any low-end hardware**.
* **AI 3D Game Generation:** Embedded artificial intelligence processing models within the engine core, supporting real-time automated trajectory calculations, schedule optimization, and dynamic aim-locking algorithms for intelligent 3D entities.
* **Hardware-Level Acceleration (Graphics Upscale):** Proprietary static mesh batching algorithms combined with optimized binary `Float32Array` buffers communicating directly with VRAM/GPU. This ensures a rock-solid 60 FPS performance, minimizes thermal throttling, and significantly reduces hardware power consumption.

### 🌐 Autonomous Multiplayer Networking & Servers
* **Dedicated Nakama Server Support:** Out-of-the-box integration with sovereign Nakama Backend server architectures. Developers can independently manage user accounts, global leaderboards, guilds, and complex MMORPG global economies.
* **Peer JS P2P Dedicated Network:** Dedicated low-latency WebRTC peer-to-peer layer powered by independent Peer JS servers, reducing ping to near-zero, eliminating packet loss, and featuring smart automated reconnection for live PvP matches.
* **Advanced Network Scripting:** Ultra-flat serialized data stream compression, delivering seamless state synchronization for multi-dimensional multiplayer instances.

### 🔎 Scripting Core & Ultimate Security
* **💻 MiaoZi JS Scripting Language:** A dedicated scripting runtime engineered from the ground up by Nguyen Hiep (XiaoYao). Features short, clean syntax with high-speed method chaining, pre-compiled macros like `.sp()`, `.spadd()`, matrix mathematics, and a built-in astronomical perpetual calendar module.
* **⚠️ Hardened Anti-Cheat Engine:** Dynamic cryptographic firewall layer blocking 100% of memory injection attempts, unauthorized VRAM tampering, god-mode exploits, item duplication, or client-side variable manipulations.

### 🗒 Frontend UI/UX Customization
* **Infinite UI Creativity via HTML & CSS:** The entire editor interface, toolbars, and context menus are built directly using HTML5 and CSS3 layouts (vw/vh, Flexbox, Grid), making UI/UX styling as flexible and beautiful as professional web design.
* **Local-First Storage (Godot-style):** Forced local file system prioritization (`Local File`) by default instead of cloud storage, ensuring absolute privacy and intellectual property protection for game developers.

---

## 🗒 Technical Architecture

MiaoZi XiaoYao Engine is modularly segregated into the following core directories for deep customization:

| Directory | ℹ️ Description |
| --------- | ------------- |
| `Core`    | Base classes defining game serialization structures and IDE management tools. |
| `GDJS`    | Core game engine runtime optimized in TypeScript, utilizing PixiJS and Three.js for 2D/3D WebGL rendering. |
| `newIDE`  | Visual editor workspace built on top of React and Electron frameworks. |

---

## 🛠️ Development Setup & Compiling

### 1. Prerequisites
* Install [Node.js](https://nodejs.org) (LTS version highly recommended).
* Install [Git](https://git-scm.com).

### 2. Dependency Installation
Open your terminal at the project root directory and execute:
```bash
cd newIDE/app
npm install

cd ../electron-app
npm install
```

### 3. Trigger Production Compilation (.exe)
Double-click the automated script located at the workspace root folder:
```cmd
AutoBuild.bat
```
*The `.bat` file is configured by Nguyen Hiep to expand hardware allocation up to 8GB RAM (`--max-old-space-size=8192`) for full-scale front-end compilation and automated security token embedding.*

The compiled binaries will be exported to `newIDE/electron-app/dist/` as a standalone installer.

---

## 🤝 License & Credits

* **Language Creator & Lead Core Engineer:** Nguyen Hiep (Born in 1999 - ADMIN MIAOZIGAME).
* **Proprietary Copyright:** Established and legally protected since August 25, 2026.
* **License:** Licensed under free open-source terms (MIT / GPL v3 compatible). You are fully authorized to use this engine to commercialize your exclusive proprietary game projects.

---

## ☕ Support Me

If you appreciate this streamlined and powerful engine runtime, feel free to buy me a coffee to fuel the development of next-generation quantum algorithms:
👉 **[Support me on Buy Me A Coffee](https://buymeacoffee.com/miao_zi_xiao_yao)**



![MiaoZi XiaoYao Engine banner](https://githubusercontent.com "MiaoZi XiaoYao Engine banner")

# 喵子逍遥引擎 (MiaoZi JS)

**喵子逍遥引擎 (MiaoZi XiaoYao Engine)** 是一款打破常规的跨平台独立游戏引擎，由核心工程师 **阮协 (Nguyen Hiep / 逍遥 / XiaoYao)**（1999年生 - **MiaoZiGame** 创始人兼独立主导者）进行深度重构与定制开发。

本引擎实现了从前端 React 架构到 Electron 容器壳体的全栈式算力优化。项目核心旨在打造一套**纯本地化、完全独立（Godot风格）**的游戏开发工作流，具备神级动态反作弊防火墙、去中心化多人联机网络底层架构以及自主可控的 3D AI 协同算力。

---

## ✨ 核心升级特性

### 📊 顶尖 3D/2D 图形与人工智能
* **完美的多平台低配优化：** 引擎的 **2D 与 3D 渲染管线均已实现完美优化，即使在极低配置的传统设备上，也能流畅运行高品质的次世代游戏画面**。
* **AI 3D 游戏生成：** 引擎内核深度植入人工智能处理模型，支持对智能 3D 实体进行实时全自动轨迹计算、日程优化和动态锁头自瞄算法。
* **硬件级高能效加速 (Graphics Upscale)：** 独创的静态网格体（Static Mesh）合批算法，配合优化的二进制 `Float32Array` 缓冲区与显存（VRAM/GPU）实现无缝高速直连。确保 60 FPS 满帧极速运行，大幅降低硬件发热，完美节省设备功耗。

### 🌐 自主联机网络与独立服务器架构
* **内置 Nakama 专属服务器支持：** 原生集成自主可控的 Nakama 后端服务器架构。允许开发者完全独立地管理玩家账户、全球排行榜（Leaderboard）、公会（Guild）以及复杂的 MMORPG 全局经济系统。
* **Peer JS P2P 专用网络：** 由独立的 Peer JS 服务器驱动 WebRTC 纯端到端（P2P）同步层，将网络延迟（Ping）降至近乎零零延迟状态，彻底消除丢包率（Packet loss），并具备针对实时 PvP 对战的智能断线重连机制。
* **高阶网络脚本技术：** 采用超扁平化序列式数据流压缩技术，实现多人在线跨维度实例的多端丝滑状态同步。

### 🔎 神级脚本核心与极限反作弊安全
* **💻 专属 MiaoZi JS 脚本语言：** 由阮协（逍遥）从零自主设计研发的轻量高能脚本运行时。语法精简利落，支持超高速方法链（Method Chaining）解析，原生集成了如 `.sp()`、`.spadd()` 等超能力宏方法，并内置矩阵高级数学运算和天文黄历万年历模块。
* **⚠️ 神级动态反作弊防火墙：** 核心级动态加密内存防火墙，100% 拦截并阻断外挂工具对显存及内存的恶意注入，从根本上杜绝客户端无敌、改数值、刷道具等篡改行为。

### 🗒 自定义客户端 UI/UX 界面
* **基于 HTML & CSS 的无限 UI 创意：** 整个编辑器工作区、工具栏及右键菜单均直接采用 HTML5 和 CSS3 现代布局（vw/vh, Flexbox, Grid）进行重构，使游戏 UI 及工具界面的定制像专业网页设计一样灵活精美。
* **默认本地化存储（Godot风格）：** 强制系统默认将工程项目直接保存至计算机本地磁盘（`Local File`），剔除强制云端束缚，绝对保护独立游戏开发者的资产隐私权与知识产权。

---

## 🗒 技术架构

喵子逍遥引擎模块化划分为以下核心目录，方便进行底层代码的干预与定制：

| Directory | ℹ️ Description |
| --------- | ------------- |
| `Core`    | 核心处理类结构，定义游戏项目的序列化架构与 IDE 管理工具。 |
| `GDJS`    | 基于 TypeScript 深度优化的核心游戏引擎，使用 PixiJS 和 Three.js 进行 2D/3D WebGL 图形渲染。 |
| `newIDE`  | 基于 React 和 Electron 框架构建的可视化编辑器工作区。 |

---

## 🛠️ 引擎自动化构建与打包指南

### 1. 环境准备
* 安装 [Node.js](https://nodejs.org) M（强烈推荐最新的 LTS 稳定版）。
* 安装 🛠 [Git](https://git-scm.com) 版本控制工具。

### 2. 依赖库一键安装
在项目根目录下打开终端，依次执行以下命令：
```bash
cd newIDE/app
npm install

cd ../electron-app
npm install
```

### 3.  kích nổ 启动自动化打包流程 (.exe)
在项目根目录下，双击运行自动化脚本：
```cmd
AutoBuild.bat
```
*该 `.bat` 批处理文件已由阮协完成高级性能配置，将硬件运存分配扩展至 8GB RAM (`--max-old-space-size=8192`)，用以支持大规模前端模块的全速编译并自动嵌入安全加密 Token。*

打包完成后，最终的独立安装包程序将输出在 `newIDE/electron-app/dist/` 目录下。

---

## 🤝 版权与开源协议

* **语言创始人兼首席核心工程师：** 阮协 (Nguyen Hiep / 1999年生 - 喵子游戏 ADMIN)。
* **自主版权所有：** 核心重构版自 2026 年 8 月 25 日起正式确立并受到版权合法保护。
* **开源许可：** 严格遵循开源自由协议（MIT / GPL v3 兼容）。您拥有完全合法的权利将本引擎用于您的商业独占游戏项目的开发与发售。

---

## ☕ 赞助与支持

如果您喜欢这款精简、高效且强悍的独立游戏引擎，欢迎请我喝杯咖啡，这将是我继续攻克下一代量子级游戏算法的强大动力：
👉 **[在 Buy Me A Coffee 上支持我](https://buymeacoffee.com/miao_zi_xiao_yao)**



![MiaoZi XiaoYao Engine banner](https://githubusercontent.com "MiaoZi XiaoYao Engine banner")

# 苗子逍遥エンジン (MiaoZi JS)

**苗子逍遥エンジン (MiaoZi XiaoYao Engine)** は、エンジニアである **グエン・ヒエップ (Nguyen Hiep / 逍遥 / XiaoYao)**（1999年生まれ - **MiaoZiGame** 代表）によってコアソースから深くカスタマイズ・開発された、限界を突破する次世代のクロスプラットフォーム・ゲームエンジンです。

本エンジンは、フロントエンドの React アーキテクチャから Electron コンテナにいたるまで、システム全体で最適化されています。クラウドの制約から脱却した**完全なローカル独立型（Godotスタイル）**のワークフローを提唱し、強力なアンチチート保護、自律型マルチプレイヤーネットワーク、そして独立した 3D AI 演算能力を備えています。

---

## ✨ 核心的な拡張機能

### 📊 最高峰の 3D/2D グラフィックスと人工知能 (AI)
* **完璧なローエンド最適化:** **2D および 3D のレンダリングパイプラインは完璧に最適化されており、スペックの低いPCや古い端末であっても、高品質なグラフィックスのゲームを非常に滑らかに動作させることができます**。
* **AI 3D ゲームジェネレーション:** エンジンコアに人工知能処理モデルを深くシームレスに統合。インテリジェントな 3D エンティティに対して、リアルタイムの自動軌道計算、スケジュール最適化、および動的なエイムロックアルゴリズムをサポートします。
* **ハードウェアレベルの高速化 (Graphics Upscale):** 独自の静的メッシュ（Static Mesh）バッチ処理アルゴリズムと、VRAM/GPU と直接高速通信するバイナリ `Float32Array` バッファの組み合わせにより、 60 FPS の安定したパフォーマンスを維持。デバイスの発熱を抑え、バッテリー消費を極限まで低減します。

### 🌐 自律型マルチプレイヤーネットワークと独立サーバー
* **Nakama 専用サーバー標準対応:** 外部に依存しない独自の Nakama バックエンドサーバーアーキテクチャとネイティブに統合。開発者はユーザーアカウント、グローバルリーダーボード、ギルド、および MMORPG の複雑な経済システムを完全に自律管理できます。
* **Peer JS P2P 専用ネットワーク:** 独立した Peer JS サーバーによって駆動する WebRTC の純粋なピアツーピア（P2P）同期層を構築。ネットワーク遅延（Ping）をほぼゼロに抑え、パケットロスを完全に排除し、リアルタイム PvP 対戦のためのスマートな自動再接続機能を備えています。
* **高度なネットワークスクリプティング:** 超フラットなシリアライズデータストリーム圧縮技術を採用し、多人数のマルチプレイヤインスタンス間で滑らかな状態同期を実現します。

### 🔎 神級スクリプトコアと究極のセキュリティ
* **💻 独自スクリプト言語「MiaoZi JS」:** グエン・ヒエップ（逍遥）がゼロから設計・開発した軽量かつ高性能なスクリプトランタイム。シンプルで簡潔な構文、超高速なメソッドチェーン（Method Chaining）解析を特徴とし、`.sp()` や `.spadd()` などの強力なマクロメソッド、マトリックス高度数学演算、および天文万年暦モジュールを標準内蔵しています。
* **⚠️ 究極のメモリ改ざん防止（アンチチート）:** コアレベルの動的暗号化メモリファイアウォール層が、外部チートツールによる VRAM やメモリへの不正なインジェクションを 100% 遮断。クライアント側での無敵化、ステータス改ざん、アイテム不正増殖などの不正行為を根本から防ぎます。

### 🗒 自由な UI/UX カスタマイズ
* **HTML5 & CSS3 による無限の表現力:** エディタのワークスペース、ツールバー、コンテキストメニューにいたるまで、HTML5 および CSS3 の現代的なレイアウト（vw/vh, Flexbox, Grid）で直接構築されています。プロのウェブデザインと同じくらい柔軟で美しい UI/UX スタイリングが可能です。
* **ローカルファーストのデフォルト保存（Godotスタイル）:** プロジェクトデータは、クラウドではなくデフォルトで常にローカルストレージ（`Local File`）に優先保存されます。独立系ゲーム開発者のデータプライバシーと知的財産権を絶対的に保護します。

---

## 🗒 技術アーキテクチャ

苗子逍遥エンジンは、ディープなカスタマイズを容易にするため、以下のコアディレクトリにモジュール化されています：

| Directory | ℹ️ Description |
| --------- | ------------- |
| `Core`    | ゲームデータの構造および IDE 管理ツールのシリアライズ構造を定義するコアクラス。 |
| `GDJS`    | TypeScript で高度に最適化されたゲームエンジンランタイム。2D/3D WebGL レンダリングに PixiJS および Three.js を採用。 |
| `newIDE`  | React と Electron フレームワークをベースに構築されたビジュアルエディタ環境。 |

---

## 🛠️ 開発環境のセットアップと自動ビルド

### 1. 前提条件
* [Node.js](https://nodejs.org) の環境（最新の LTS 安定版を強く推奨）。
* [Git](https://git-scm.com) バージョン管理ツール。

### 2. 依存関係のインストール
プロジェクトのルートディレクトリでターミナルを開き、以下のコマンドを実行します：
```bash
cd newIDE/app
npm install

cd ../electron-app
npm install
```

### 3. 🛠 自動ビルドの実行 (.exe)
ワークスペースのルートフォルダにある自動化スクリプトを実行（ダブルクリック）します：
```cmd
AutoBuild.bat
```
*この `.bat` ファイルは、グエン・ヒエップによってハードウェア割り当てを 8GB RAM (`--max-old-space-size=8192`) まで拡張するように調整されており、大規模なビルドを最高速で処理し、セキュリティ暗号化トークンを自動で組み込みます。*

ビルドが完了すると、独立したインストーラー形式のバイナリが `newIDE/electron-app/dist/` ディレクトリに出力されます。

---

## 🤝 ライセンスと知的財産権

* **言語開発者 兼 開発総責任者:** グエン・ヒエップ (Nguyen Hiep / 1999年生まれ - MiaoZiGame 代表)。
* **独占的著作権:** 2026年8月25日より正式に確立され、法的保護下にあります。
* **ライセンス:** オープンソースライセンス（MIT / GPL v3 互換）に準拠しています。このゲームエンジンを使用して、ご自身の商業的な独占ゲームプロジェクトを自由に開発・販売する権利が完全に認められています。

---

## ☕ 開発者をサポート

この洗練された強力なゲームエンジンを気に入っていただけましたら、次世代の量子レベルゲームアルゴリズム開発への活力として、コーヒーを1杯ご馳走していただけると励みになります：
👉 **[Buy Me A Coffee で私をサポートする](https://buymeacoffee.com/miao_zi_xiao_yao)**



