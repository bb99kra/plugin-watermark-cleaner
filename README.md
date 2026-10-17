# 🛡️ Nguyendzvn Suite - Minecraft Plugin Leak & Watermark Purger

> **100% Client-Side • Chạy Trực Tiếp Tại Trình Duyệt • Không Dùng AI • Bảo Toàn Bytecode JVMS §4.4.7**
> 
> Chuyên dụng quét và khử sạch triệt để **NulledVault, BlackSpigot, GLeaks, DirectLeaks, Buyer ID, Spigot/Polymart Tokens, Telemetry Phone-Home, Zip Archive Comments** và bảo vệ an toàn danh tính 100% mà không làm hỏng plugin.

---

## 🌐 Trải Nghiệm Trực Tiếp (Live Demo)

👉 **Website chính thức:** [https://bb99kra.github.io/plugin-watermark-cleaner/](https://bb99kra.github.io/plugin-watermark-cleaner/)

---

## 🌟 Tính Năng Tiến Hóa Cấp Doanh Nghiệp (Enterprise Features)

### 1. ⚡ Chế Độ (pure) Standalone Engine (Độc Lập Tuyệt Đối)
- **1-Click Pure Conversion**: Chỉ với 1 thao tác, tự động biến mọi file `.jar` thành bản độc lập hoàn chỉnh.
- **Vô hiệu hóa kiểm tra DRM nhị phân**: Hóa giải các cơ chế kiểm tra bản quyền ngầm, bypass lỗi `IllegalStateException` (GLeaks, Nexo AES-CBC traps, Songoda, Polymart).
- **Cắt đứt toàn bộ Telemetry & Phone-Home**: Tự động chuyển hướng toàn bộ request gọi về server từ xa (`api.spigotmc.org`, `polymart.org/api`, `songoda.com/api`, `pstats.devs.beer`, `license.*`, `nulledvault.com`) về loopback dummy `127.0.0.1`.
- **Tự động xuất xưởng file**: Đóng gói chuẩn hóa và tải về ngay với tên `<Plugin>-Pure.jar`.

### 2. 🛡️ Security Auditor & Watermark Sanitizer
- **Thang điểm bảo mật doanh nghiệp**: Đánh giá cấp độ rủi ro (**A+, A, B, D, F**) và đo lường tỷ lệ nguy cơ (% Risk Score).
- **Phát hiện Buyer ID**: Tự động bóc tách các dãy số User ID được nhúng ngầm trong class bytecode kèm đường dẫn hồ sơ SpigotMC tương ứng.
- **Xóa sạch Zip Archive Comment**: Quét và dọn sạch ghi chú nén của file (như `User: HoYeuEmBangMat`, `GLeaks.pro`, `NulledVault`).
- **Làm sạch MANIFEST.MF**: Gỡ bỏ các header `Spigot-User-Id`, `BuiltByBit-Id`, `Polymart-Id`, `Buyer`, `Nonce`.
- **Triệt tiêu Console Banners**: Xóa bỏ các dòng thông báo leaker in ra console khi bật plugin (hỗ trợ cả Plain Text lẫn chuỗi mã hóa **Base64**).
- **Chuẩn hóa Timestamps**: Xóa dấu vết thời gian tải về (Zero-metadata footprint).

### 3. 🔍 Bytecode Constant Pool Inspector
- Soi trực tiếp constant pool nhị phân của hàng nghìn class trong file JAR ngay tại trình duyệt.
- Tìm kiếm từ khóa nhanh chóng (như `license`, `spigot`, `gleaks`, `http`, `user_id`).

### 4. 🔒 Bảo Mật 100% Tại Client (Zero-Server Architecture)
- Hoạt động 100% trong bộ nhớ RAM trình duyệt thông qua **JSZip** và bộ mã hóa **Oracle JVMS §4.4.7 Modified UTF-8 (MUTF-8)**.
- **File không bao giờ bị upload lên bất kỳ máy chủ nào!**
- Hoạt động trơn tru vĩnh viễn trên GitHub Pages mà không tốn chi phí máy chủ.

---

## 🚀 Hướng Dẫn Sử Dụng Cục Bộ (Offline)

Chỉ cần tải file `index.html` và `jszip.min.js` về máy và mở bằng bất kỳ trình duyệt nào (Chrome, Edge, Firefox, Brave, Safari) là có thể sử dụng ngay mà không cần internet!

---

## 📜 Bản Quyền & Giấy Phép
Phát triển bởi **Nguyendzvn & Antigravity Suite**. Mã nguồn mở theo giấy phép MIT.
