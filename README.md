# 💻 Tên đề tài: Xây dựng Website Thương mại Điện tử Smart PC Hub

## 📖 Giới thiệu website/hệ thống
**Smart PC Hub** là nền tảng thương mại điện tử chuyên biệt cung cấp PC Gaming cao cấp và linh kiện máy tính. Hệ thống được xây dựng với mục tiêu mang lại trải nghiệm mua sắm mượt mà, giao diện mang phong cách công nghệ hiện đại (Premium Tech UI) có độ tương phản cao. 

Các tính năng nổi bật của hệ thống bao gồm:
* Quản lý sản phẩm, danh mục và đơn hàng tự động.
* Tìm kiếm sản phẩm thời gian thực (Real-time AJAX Search).
* Tích hợp cổng thanh toán trực tuyến qua mã QR tự động (PayOS).
* Giao diện tùy biến sâu bằng CSS thuần, tối ưu hóa hiển thị trên nhiều thiết bị.

## 👥 Danh sách thành viên & Phân công nhiệm vụ

| STT | Họ và tên thành viên | Mã số sinh viên (MSSV) | Phân công nhiệm vụ cụ thể | Mức độ hoàn thành |
|:---:|:---|:---:|:---|:---:|
| 1 | [Đàm Văn Sơn - Nhóm trưởng] | [MSSV 23810310069] | [ Quản lý dự án, Thiết kế Database, Tích hợp API Thanh toán PayOS] | 100% |
| 2 | [Nguyễn Văn Thắng] | [MSSV 23810310058] | [Xây dựng cấu trúc HTML/CSS, Tối ưu giao diện Custom UI, Quản lý Layout] | 100% |
| 3 | [Phạm Văn Tường] | [MSV 23810310058] | [Cấu hình WooCommerce, Xử lý tính năng Tìm kiếm FiboSearch, Quản trị hệ thống] | 100% |

## 🛠️ Công nghệ sử dụng
* **Nền tảng lõi (Core Framework):** WordPress 6.x
* **Nền tảng thương mại điện tử:** WooCommerce
* **Ngôn ngữ phát triển:** PHP 8.x, JavaScript, HTML5, CSS3 Custom (Flexbox, Glassmorphism UI)
* **Hệ quản trị cơ sở dữ liệu:** MySQL / MariaDB
* **API & Plugin tích hợp:**
  * Cổng thanh toán: PayOS API
  * Tìm kiếm động: FiboSearch (AJAX)
* **Môi trường & Mạng:** Docker (Localhost), Ngrok (Tạo Tunnel Public)

## ⚙️ Hướng dẫn cài đặt
Để cài đặt hệ thống trên môi trường Localhost, vui lòng thực hiện các bước sau:

1. **Chuẩn bị môi trường:** Cài đặt phần mềm Doker. Khởi động module Apache và MySQL.
2. **Clone mã nguồn:**
   Tải mã nguồn về hoặc dùng lệnh git:
   ```bash
   git clone [[Nhập link Github Repository của nhóm bạn](https://github.com/SonDamNH/smartpchub-core)]
   chạy git bash hoặc trong terminal lệnh để khời động server: ngrok http --domain=nociceptive-krysta-egoistically.ngrok-free.dev 80

link sản phẩm:https://nociceptive-krysta-egoistically.ngrok-free.dev/
tài khoản demo: tài khoản: adimpchub
                mk:123admin
   
