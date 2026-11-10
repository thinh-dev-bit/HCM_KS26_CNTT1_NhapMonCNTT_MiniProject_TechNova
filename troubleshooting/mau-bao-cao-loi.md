# Quy trình Troubleshooting 4 Chặng & Mẫu Báo Cáo Lỗi (Bug Report)

## 1. Quy trình Tự xử lý 80% Sự cố
- **Chặng 1 (Googling đúng cách):** Bóc tách lỗi nguyên văn, dùng toán tử `site:stackoverflow.com`, dấu ngoặc kép `""` và dấu trừ `-`.
- **Chặng 2 (Community Search):** Kiểm tra GitHub Issues (Open/Closed), ưu tiên đọc bình luận có `Thumbs Up (👍)` cao và tìm kiếm `Workaround`.
- **Chặng 3 (AI Decoding):** Dùng Prompt 3 thành phần (Ngữ cảnh ➔ Lỗi nguyên văn ➔ Yêu cầu). **Cấm** gửi API Key / Secrets lên AI.
- **Chặng 4 (Bug Report Framework):** Nếu sau 15 phút không tự gỡ được, lập tức gửi yêu cầu hỗ trợ theo mẫu chuẩn dưới đây.

---

## 2. Mẫu Bug Report Chuẩn 4 Mảnh ghép (Bắt buộc khi nhờ IT Support)

###  [BUG REPORT - TECHNOVA HELPDESK]
--------------------------------------------------
**1. Context (Ngữ cảnh môi trường):**
- Hệ điều hành: [Ví dụ: Windows 11 Pro / macOS Sonoma]
- Môi trường thực thi: [Ví dụ: VS Code Terminal / Docker v27]
- Tác vụ đang làm: [Ví dụ: Chạy lệnh `npm run dev` để khởi động frontend]

**2. Expected (Hành vi mong muốn):**
- Hệ thống hiển thị gì khi chạy đúng? [Ví dụ: Ứng dụng chạy thành công tại http://localhost:3000]

**3. Actual (Kết quả thực tế / Hiện tượng lỗi):**
- Hệ thống trả về lỗi gì? [Ví dụ: Lỗi không tìm thấy module hoặc xung đột cổng port]

**4. Log & Screenshot (Nhật ký lỗi & Hình ảnh minh họa):**
- Nguyên văn dòng Error Log từ Terminal:
\`\`\`text
[Dán 3-5 dòng lỗi nguyên văn tại đây - Đã che thông tin nhạy cảm]
\`\`\`
- Các bước Troubleshooting đã thử: [Ví dụ: Đã kiểm tra node_modules, đã thử đổi cổng nhưng vẫn lỗi...]
--------------------------------------------------