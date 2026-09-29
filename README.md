# EncyAuth – Trình xác thực 2 bước

**EncyAuth** là ứng dụng web hiện đại (PWA) giúp bạn lưu trữ và quản lý mã xác thực 2 bước (2FA/TOTP) an toàn. Được xây dựng dựa trên kiến trúc **Zero-Knowledge**, toàn bộ dữ liệu mã bí mật của bạn sẽ được mã hóa trực tiếp trên thiết bị trước khi đồng bộ lên đám mây. Điều này đảm bảo không một ai — kể cả nhà phát triển — có thể giải mã và đọc được thông tin của bạn.

🌐 **Trải nghiệm ngay tại:** [https://encyauth.github.io/](https://encyauth.github.io/)

## ✨ Tính năng nổi bật

- 🔐 **Bảo mật tối đa:** Dữ liệu Secret Key được mã hóa bằng thuật toán AES-GCM 256-bit kết hợp với Khóa bảo vệ dữ liệu (DEK).
- 📶 **Hoạt động ngoại tuyến (Offline):** Thoải mái xem mã TOTP 6 số, thêm, sửa hoặc xóa dịch vụ ngay cả khi mất kết nối mạng. Ứng dụng sẽ tự động đồng bộ mọi thay đổi ngay khi có mạng trở lại.
- ☁️ **Đồng bộ đám mây thông minh:** Dữ liệu mã hóa được lưu trữ an toàn qua hệ thống Firebase. Bạn có thể dễ dàng quản lý, tải về hoặc khôi phục các bản sao lưu đồng bộ xuyên suốt các thiết bị cá nhân.
- 📱 **Trải nghiệm liền mạch (PWA):** Cài đặt trực tiếp lên màn hình chính của iOS, Android và Desktop để sử dụng mượt mà, tiện lợi như một ứng dụng gốc (native app).
- 🛠 **Bộ công cụ tích hợp:** Tự động tính toán chu kỳ thời gian làm mới mã TOTP. Sao lưu và khôi phục dữ liệu linh hoạt qua file JSON kèm theo thông tin phiên bản và số lượng dịch vụ trực quan.
- 🛡 **Chống truy cập trái phép:** Hệ thống sẽ tự động khóa và hiển thị đếm ngược thời gian chờ nếu phát hiện người lạ cố tình nhập sai Mật khẩu chính nhiều lần.

## 🛠 Công nghệ sử dụng

- **Giao diện (Frontend):** HTML5, JavaScript (ES6+), Tailwind CSS, Lucide Icons, OTPAuth Library
- **Hệ thống (Backend & DB):** Firebase Auth (Đăng nhập Google), Firebase Firestore, Firebase Cloud Storage, Firebase Cloud Functions
- **Nền tảng (PWA):** Service Worker (Xử lý Offline), Web App Manifest
- **Bảo mật:** Web Crypto API (PBKDF2, AES-GCM)

## ⚠️ Lưu ý bảo mật quan trọng

- Hệ thống **TUYỆT ĐỐI KHÔNG** lưu trữ *Mật khẩu chính (Master Password)* của bạn. 
- Nếu quên Mật khẩu chính, bạn sẽ **mất vĩnh viễn quyền truy cập** vào kho dữ liệu của mình. Hãy chắc chắn rằng bạn đã ghi nhớ thật kỹ hoặc lưu giữ mật khẩu này ở một nơi an toàn trước khi sử dụng.

## 👨‍💻 Tác giả

Phát triển bởi **Hoàng Đợi**.