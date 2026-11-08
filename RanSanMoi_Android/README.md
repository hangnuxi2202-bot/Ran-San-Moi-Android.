# Rắn Săn Mồi — Android APK

Dự án Android WebView đóng gói trò chơi HTML hiện tại. Game được nhúng trong `app/src/main/assets/index.html`, chạy trực tiếp trên điện thoại và không cần kết nối mạng sau khi cài.

## Tạo APK bằng GitHub Actions
1. Tạo một repository GitHub mới.
2. Giải nén toàn bộ ZIP này và tải toàn bộ nội dung lên repository (giữ nguyên thư mục `.github`).
3. Mở tab **Actions** → chọn **Build Android APK** → **Run workflow**.
4. Khi chạy xong, mở lượt chạy mới nhất, kéo xuống **Artifacts** và tải `Ran-San-Moi-APK`.
5. Giải nén artifact, lấy `app-debug.apk`, gửi sang điện thoại Android và cài đặt. Nếu máy hỏi, cho phép cài ứng dụng từ nguồn này.

## Build bằng Android Studio
Mở thư mục dự án này trong Android Studio, chờ Gradle Sync, sau đó chọn **Build → Build Bundle(s) / APK(s) → Build APK(s)**.

- Package: `vn.ransanmoi.game`
- Minimum Android: Android 6.0 (API 23)
- APK đầu ra: `app/build/outputs/apk/debug/app-debug.apk`

Lưu ý: đây là bản debug để cài thử, chưa phải APK phát hành ký số.
