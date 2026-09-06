# 🛡️ Minecraft Plugin Watermark & User Info Sanitizer

> **100% Client-Side • Chạy Vĩnh Viễn Không Cần Server • Bảo Mật Tuyệt Đối**
> 
> Công cụ phân tích và khử sạch triệt để **Watermark danh tính người dùng (User ID), Buyer ID, Phone-home và Console Banners** từ các nền tảng: **SpigotMC, BuiltByBit (MC-Market), Polymart, Songoda & NulledVault**.

---

## 🌟 Điểm Nổi Bật (Key Features)

### 1. 🟠 SpigotMC Watermarks
- Tự động phát hiện và triệt tiêu **User ID** (e.g. `2128446`) bị Spigot nhúng ngầm trong class bytecode.
- Neutralize các placeholder của Spigot: `%%__USER__%%`, `%%__RESOURCE__%%`, `%%__NONCE__%%`, `%%__USERNAME__%%`.
- Cắt đứt các cuộc gọi Spigot API Phone-home:
  - `https://api.spigotmc.org/simple/0.2/index.php?action=getAuthor&id=...` (Ngăn server tự động kéo tên tài khoản Spigot về in lên console).
  - `https://api.spigotmc.org/legacy/premium.php?user_id=...` (Ngăn verify license ngầm).

### 2. 🟣 BuiltByBit (MC-Market) & Polymart
- Loại bỏ các header `BuiltByBit-User-Id`, `BBB-Resource-Id`, `Polymart-User-Id`, `Buyer`, `Nonce` trong `META-INF/MANIFEST.MF`.
- Vô hiệu hóa các token `%%__POLYMART__%%` và API tracking.

### 3. 📁 Zip Comment & File Metadata (NulledVault, Leaks...)
- Quét và xóa sạch **Zip Archive Comment** (như watermark `User: HoYeuEmBangMat`, `NulledVault download...`).
- Xóa các file chữ ký điện tử `.SF`, `.RSA`, `.DSA` và file rác `.spigot`, `.builtbybit`, `__MACOSX/`.
- Chuẩn hóa ngày sửa đổi (Timestamps) về mốc cố định để chống truy vết thời gian tải (timestamp correlation).

### 4. 📢 Console Banners & Quảng Cáo Trong Bytecode
- Quét và triệt tiêu các thông báo in ra console khi bật plugin (`Cracked by...`, `Leaked by...`).
- Tự động giải mã và xóa sạch các chuỗi **Base64** giấu banner console.

### 5. 🔒 100% Riêng Tư Tại Client (Client-Side Only)
- Chạy trực tiếp trong trình duyệt thông qua **JSZip** và bộ phân tích nhị phân **Java Bytecode Constant Pool**.
- **File không bao giờ bị upload lên bất kỳ server nào!**
- Không tốn chi phí hosting, hoạt động vĩnh viễn trên GitHub Pages.

---

## 🚀 Hướng Dẫn Kích Hoạt Miễn Phí Trên GitHub Pages (Chạy Vĩnh Viễn)

1. **Tạo repository mới trên GitHub**:
   - Tên repo: `plugin-watermark-cleaner` (hoặc tên tùy thích).
   - Chọn chế độ **Public**.

2. **Đẩy mã nguồn lên**:
   ```bash
   git init
   git add .
   git commit -m "feat: initial release of plugin watermark cleaner"
   git branch -M main
   git remote add origin https://github.com/<tai-khoan-cua-ban>/plugin-watermark-cleaner.git
   git push -u origin main
   ```

3. **Bật GitHub Pages**:
   - Vào **Settings** của repository trên GitHub.
   - Chọn mục **Pages** ở thanh menu bên trái.
   - Tại mục **Build and deployment -> Source**, chọn **Deploy from a branch**.
   - Branch: chọn **`main`**, folder: **`/ (root)`** -> Bấm **Save**.

4. **Tận hưởng tên miền vĩnh viễn**:
   - Sau 1 phút, website của bạn sẽ hoạt động trực tiếp tại:
     `https://<tai-khoan-cua-ban>.github.io/plugin-watermark-cleaner/`
   - Hỗ trợ gán tên miền riêng miễn phí (Custom domain CNAME) bất kỳ lúc nào!

---

## 💻 Chạy Trực Tiếp Offline / Cục Bộ

Bạn chỉ cần mở trực tiếp file `index.html` bằng bất kỳ trình duyệt nào (Chrome, Firefox, Safari, Edge) là sử dụng được ngay lập tức mà không cần cài đặt thêm bất kỳ phần mềm hay server nào!

---

## 📜 Giấy Phép & Bản Quyền
Phát triển bởi **Nguyendzvn & Antigravity Suite**. Mã nguồn mở theo giấy phép MIT.
