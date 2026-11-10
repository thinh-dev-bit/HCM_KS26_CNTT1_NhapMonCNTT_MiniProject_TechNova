# Cấu hình Môi trường Trình duyệt Chuyên nghiệp & Đa Profile

## 1. Phân tách Đa Profile (Data Isolation)
Nhân viên mới bắt buộc phải tạo và duy trì tối thiểu 2 Profile độc lập trên Google Chrome / Edge:
- **Profile 1 (Personal):** Dùng cho mục đích cá nhân, giải trí, mạng xã hội cá nhân.
- **Profile 2 (TechNova_Work):** Dùng riêng cho công việc tại công ty, đăng nhập Email công ty, GitHub, AWS, Jira. 
*Nguyên lý:* Không dùng chung Profile để tránh rò rỉ Cookies/Session cá nhân sang môi trường doanh nghiệp.

## 2. Quản lý Bookmark Manager
Sắp xếp Bookmark thành 3 thư mục cốt lõi:
1. `01_Work_Dev`: GitHub Repo, Jira Board, AWS Console, Staging Environment.
2. `02_Onboarding_Docs`: Tài liệu nội bộ TechNova, SRS Onboarding Kit, Wiki công ty.
3. `03_Tools`: Trình quản lý mật khẩu Bitwarden Web, ChatGPT, Google Meet, công cụ format code.

## 3. Cài đặt Extension & Giới hạn Quyền (Site Access)
- **Dev Suite:** React DevTools, JSON Formatter.
- **Productivity Suite:** Grammarly, uBlock Origin (chặn quảng cáo độc hại).
- **Security Suite:** Bitwarden Password Manager extension.
- **Quy tắc Site Access:** Đặt quyền truy cập của mọi extension ở chế độ **"On click"** (Chỉ khi nhấp vào icon) thay vì "On all sites" để bảo vệ dữ liệu duyệt web.

## 4. Kỹ thuật DevTools F12 Cơ bản
- **Inspect Element:** Nhấn `F12` hoặc `Ctrl+Shift+I` để kiểm tra giao diện, debug lỗi JavaScript console.
- **Phân biệt Cache & Cookies:** Vào thẻ *Application* để xóa Storage/Cookies khi giao diện bị kẹt phiên bản cũ.
- **Hard Reload:** Nhấn `Ctrl + Shift + R` (hoặc `Cmd + Shift + R` trên Mac) để ép trình duyệt tải lại hoàn toàn tài nguyên mới từ server, bỏ qua bộ nhớ đệm.