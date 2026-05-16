# 💻 Tên đề tài: Xây dựng Website Thương mại Điện tử Smart PC Hub

## 📖 Giới thiệu website/hệ thống
**Smart PC Hub** là nền tảng thương mại điện tử chuyên biệt cung cấp PC Gaming cao cấp và linh kiện máy tính. Hệ thống được xây dựng với mục tiêu mang lại trải nghiệm mua sắm mượt mà, giao diện mang phong cách công nghệ hiện đại (Premium Tech UI) có độ tương phản cao. 

Các tính năng nổi bật của hệ thống bao gồm:
* Quản lý sản phẩm, danh mục và đơn hàng tự động.
* Tìm kiếm sản phẩm thời gian thực (Real-time AJAX Search).
* Tích hợp cổng thanh toán trực tuyến qua mã QR tự động (PayOS).
* Giao diện tùy biến sâu bằng CSS thuần, tối ưu hóa hiển thị trên nhiều thiết bị.

## 👥 Danh sách thành viên, MSSV & Phân công nhiệm vụ cụ thể

| STT | Họ và tên thành viên | Mã số sinh viên (MSSV) | Phân công nhiệm vụ cụ thể | Mức độ hoàn thành |
|:---:|:---|:---:|:---|:---:|
| 1 | Đàm Văn Sơn (Nhóm trưởng) | 23810310069 | Quản lý dự án, Thiết kế Database, Tích hợp API Thanh toán PayOS | 100% |
| 2 | Nguyễn Văn Thắng | 23810310058 | Xây dựng cấu trúc HTML/CSS, Tối ưu giao diện Custom UI, Quản lý Layout | 100% |
| 3 | Phạm Văn Tường | 23810310058 | Cấu hình WooCommerce, Xử lý tính năng Tìm kiếm FiboSearch, Quản trị hệ thống | 100% |

## 🛠️ Công nghệ sử dụng
* **Core Framework:** WordPress 6.x
* **E-commerce Engine:** WooCommerce
* **Frontend:** HTML5, CSS3 Custom (Flexbox, Glassmorphism UI)
* **Backend/Database:** PHP 8.x, MySQL/MariaDB
* **Môi trường & Triển khai (DevOps):** Docker & Docker Compose (Containerization)
* **API & Plugin tích hợp:** PayOS API (Thanh toán QR), FiboSearch (AJAX Search)
* **Network Tunnel:** Ngrok (Secure Introspectable Tunnels)

## ⚙️ Hướng dẫn cài đặt
Hệ thống được đóng gói hoàn toàn bằng Docker, giúp loại bỏ triệt để lỗi xung đột môi trường giữa các máy cục bộ.

1. **Chuẩn bị môi trường:** Máy tính cần cài đặt sẵn **Docker Desktop** (hoặc Docker Engine & Docker Compose).
2. **Clone mã nguồn:** Mở Terminal (hoặc Git Bash) và chạy chuỗi lệnh sau để tải mã nguồn và di chuyển vào thư mục dự án:

```bash
git clone [https://github.com/SonDamNH/smartpchub-core.git](https://github.com/SonDamNH/smartpchub-core.git)
cd smartpchub-core
▶️ Hướng dẫn chạy project
Tại thư mục gốc smartpchub-core, chạy lệnh sau để build các container và khởi chạy hệ thống ở chế độ chạy ngầm:

Bash
docker-compose up -d
Sau khi Docker khởi chạy thành công, hệ thống Web và Cơ sở dữ liệu sẽ tự động hoạt động và kết nối với nhau.

Để kích hoạt cổng thanh toán nhận diện Webhook phản hồi từ API ngân hàng, mở một cửa sổ Terminal mới và chạy lệnh khởi tạo đường hầm mạng Ngrok trỏ về cổng dịch vụ:

Bash
ngrok http 80
🔑 Tài khoản demo
Tài khoản Quản trị viên (Admin):

Tên đăng nhập: adimpchub

Mật khẩu: 123admin

🔗 Link online đã deploy
Đường dẫn sản phẩm thử nghiệm (Live Deploy qua Ngrok Tunnel): https://nociceptive-krysta-egoistically.ngrok-free.dev/
📺 Link video demo
Liên kết xem Video Demo thuyết minh chi tiết dự án:https://drive.google.com/file/d/1DB8DKB-7OrUr0Dgxb8hfImYCm7BZAOI9/view
