# Checklist An toàn Thông tin & Bảo mật Cá nhân

- [ ] **Bitwarden Vault:** Đã thiết lập Master Password mạnh (>= 16 ký tự, không trùng lặp).
- [ ] **Mật khẩu cá nhân:** Tuân thủ nguyên tắc 1 tài khoản - 1 mật khẩu do Password Generator sinh ra.
- [ ] **Xác thực 2FA (TOTP):** Đã kích hoạt Google/Microsoft Authenticator cho GitHub và Email công ty; tuyệt đối không dùng SMS OTP.
- [ ] **Mã khôi phục (Backup Codes):** Đã lưu trữ bộ 10 mã khôi phục an toàn trong Bitwarden Vault.
- [ ] **Phòng chống Phishing & Crack:** 
  - Luôn kiểm tra kỹ tên miền (tránh Typosquatting như `githúb.com`).
  - Áp dụng **Quy tắc 5 KHÔNG**: Không bấm link lạ, không tải phần mềm crack, không tắt Windows Defender, không dùng chung mật khẩu, không gửi Secret lên AI.
- [ ] **Bảo vệ Secrets:** Kiểm tra kỹ tệp `.env` đã được khai báo trong `.gitignore` trước khi thực hiện `git push`.