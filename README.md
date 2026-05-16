# 💻 Smart PC Hub — Website Thương mại Điện tử PC Gaming
 
<div align="center">
![Smart PC Hub Banner](./screenshots/banner.png)
 
[![WordPress](https://img.shields.io/badge/WordPress-6.x-21759B?style=for-the-badge&logo=wordpress)](https://wordpress.org/)
[![WooCommerce](https://img.shields.io/badge/WooCommerce-Latest-96588A?style=for-the-badge&logo=woocommerce)](https://woocommerce.com/)
[![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker)](https://www.docker.com/)
[![PHP](https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php)](https://www.php.net/)
 
</div>
---
 
## 📖 Giới thiệu hệ thống
 
**Smart PC Hub** là nền tảng thương mại điện tử chuyên biệt cung cấp PC Gaming cao cấp và linh kiện máy tính. Hệ thống được xây dựng với mục tiêu mang lại trải nghiệm mua sắm mượt mà, giao diện mang phong cách công nghệ hiện đại **(Premium Tech UI)** với độ tương phản cao.
 
### ✨ Tính năng nổi bật
 
- 🛒 **Quản lý sản phẩm & đơn hàng** — Quản lý danh mục, sản phẩm và toàn bộ vòng đời đơn hàng tự động qua WooCommerce.
- 🔍 **Tìm kiếm thời gian thực** — Tích hợp FiboSearch với Real-time AJAX, kết quả hiển thị tức thì không cần tải lại trang.
- 💳 **Thanh toán QR tự động** — Tích hợp cổng thanh toán PayOS, tự động sinh mã QR và xác nhận đơn hàng qua Webhook.
- 🎨 **Giao diện tùy biến sâu** — CSS thuần với Flexbox và hiệu ứng Glassmorphism, tối ưu hiển thị đa thiết bị (Responsive).
- 🐳 **Triển khai Docker** — Toàn bộ hệ thống được container hóa, không xung đột môi trường giữa các máy.
---
 
## 👥 Danh sách thành viên & Phân công nhiệm vụ
 
| STT | Họ và tên | MSSV | Phân công nhiệm vụ | Hoàn thành |
|:---:|:---|:---:|:---|:---:|
| 1 | **Đàm Văn Sơn** *(Nhóm trưởng)* | 23810310069 | Quản lý dự án, Thiết kế Database, Tích hợp API Thanh toán PayOS | ✅ 100% |
| 2 | **Nguyễn Văn Thắng** | 23810310058 | Xây dựng cấu trúc HTML/CSS, Tối ưu giao diện Custom UI, Quản lý Layout | ✅ 100% |
| 3 | **Phạm Văn Tường** | 23810310058 | Cấu hình WooCommerce, Xử lý tính năng FiboSearch, Quản trị hệ thống | ✅ 100% |
 
---
 
## 🛠️ Công nghệ sử dụng
 
| Nhóm | Công nghệ |
|:---|:---|
| **Core Framework** | WordPress 6.x |
| **E-commerce Engine** | WooCommerce |
| **Frontend** | HTML5, CSS3 Custom (Flexbox, Glassmorphism UI) |
| **Backend / Database** | PHP 8.x, MySQL / MariaDB |
| **DevOps / Triển khai** | Docker & Docker Compose (Containerization) |
| **API & Plugin** | PayOS API (Thanh toán QR), FiboSearch (AJAX Search) |
| **Network Tunnel** | Ngrok (Secure Introspectable Tunnels) |
 
---
 
## ⚙️ Hướng dẫn cài đặt
 
> Hệ thống được đóng gói hoàn toàn bằng Docker, loại bỏ triệt để lỗi xung đột môi trường giữa các máy cục bộ.
 
### Yêu cầu môi trường
 
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) (Windows / macOS) hoặc Docker Engine + Docker Compose (Linux)
- [Git](https://git-scm.com/)
- [Ngrok](https://ngrok.com/) *(chỉ cần nếu muốn kích hoạt Webhook thanh toán)*
### Các bước cài đặt
 
**Bước 1 — Clone mã nguồn về máy:**
 
```bash
git clone https://github.com/SonDamNH/smartpchub-core.git
cd smartpchub-core
```
 
**Bước 2 — Khởi chạy toàn bộ hệ thống bằng Docker:**
 
```bash
docker-compose up -d
```
 
Sau khi lệnh chạy xong, Docker sẽ tự động build các container (WordPress + MySQL) và kết nối chúng với nhau. Truy cập hệ thống tại: `http://localhost`
 
**Bước 3 *(Tùy chọn)* — Kích hoạt Webhook thanh toán PayOS qua Ngrok:**
 
Mở một cửa sổ Terminal mới và chạy:
 
```bash
ngrok http 80
```
 
Sao chép URL `https://` mà Ngrok cấp, sau đó cập nhật vào phần cấu hình **PayOS Webhook URL** trong trang quản trị WordPress.
 
---
 
## ▶️ Hướng dẫn chạy project
 
```bash
# Khởi chạy toàn bộ hệ thống ở chế độ nền (detached mode)
docker-compose up -d
 
# Xem log realtime của các container
docker-compose logs -f
 
# Dừng toàn bộ hệ thống
docker-compose down
```
 
---
 
## 🔑 Tài khoản demo
 
| Vai trò | Tên đăng nhập | Mật khẩu |
|:---:|:---:|:---:|
| 🔧 Quản trị viên (Admin) | `adimpchub` | `123admin` |
 
> ⚠️ **Lưu ý:** Đây là tài khoản demo cho mục đích kiểm thử. Vui lòng không thay đổi cấu hình hệ thống.
 
---
 
## 🖼️ Hình ảnh minh họa hệ thống
 
 
### Trang chủ
![Trang chủ Smart PC Hub](./screenshots/homepage.png)
 
### Trang sản phẩm
![Trang sản phẩm](./screenshots/product-page.png)
 
### Trang thanh toán QR (PayOS)
![Thanh toán PayOS](./screenshots/checkout-payos.png)
 
### Trang quản trị (Admin Dashboard)
![Admin Dashboard](./screenshots/admin-dashboard.png)
 
---
 
## 📺 Video Demo
 
[![Xem Video Demo](https://img.shields.io/badge/▶%20Xem%20Video%20Demo-Google%20Drive-4285F4?style=for-the-badge&logo=googledrive)](https://drive.google.com/file/d/1DB8DKB-7OrUr0Dgxb8hfImYCm7BZAOI9/view)
 
> Video demo thuyết minh chi tiết toàn bộ tính năng và luồng sử dụng của hệ thống Smart PC Hub.
 
---
 
## 🔗 Đường dẫn deploy (Live Demo)
 
> 🌐 **Live Deploy qua Ngrok Tunnel:**
>
> **[https://nociceptive-krysta-egoistically.ngrok-free.app/](https://nociceptive-krysta-egoistically.ngrok-free.dev/)**
>
> ⚠️ *Lưu ý: URL Ngrok Free có thể thay đổi sau mỗi lần khởi động lại tunnel. Nếu link không hoạt động, vui lòng liên hệ nhóm để lấy URL mới nhất.*
 
---
 
## 📁 Cấu trúc thư mục dự án
 
```
smartpchub-core/
├── docker-compose.yml       # Cấu hình Docker orchestration
├── wordpress/               # Mã nguồn WordPress & theme/plugin tùy chỉnh
│   ├── wp-content/
│   │   ├── themes/          # Theme tùy chỉnh Smart PC Hub
│   │   └── plugins/         # Các plugin: WooCommerce, FiboSearch, PayOS...
├── mysql/                   # Dữ liệu MySQL (volume mount)
├── screenshots/             # Ảnh minh họa hệ thống (dùng cho README)
└── README.md
```
 
---
 
<div align="center">
**Smart PC Hub** — *Được xây dựng với ❤️ bởi nhóm 15!
 
</div>
