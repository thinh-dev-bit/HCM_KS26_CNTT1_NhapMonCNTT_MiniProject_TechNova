# Hướng dẫn Tổ chức Không gian Cộng tác Đám mây & Phân quyền


## 1. Mô hình Hybrid Workflow (Cục bộ & Đám mây)
- **Local First (Ưu tiên cục bộ):** Mọi tài liệu, mã nguồn và tài nguyên khi đang soạn thảo/phát triển đều được lưu trữ và xử lý trực tiếp trên ổ cứng Local (SSD) của máy tính nhân viên để đảm bảo tốc độ đọc/ghi tối đa, không bị phụ thuộc vào độ trễ mạng.
- **Auto Sync (Đồng bộ tự động):** Sử dụng ứng dụng *Google Drive for Desktop* để cấu hình tự động đồng bộ ngầm các thư mục làm việc lên đám mây theo thời gian thực, giúp sao lưu an toàn và phòng tránh tuyệt đối rủi ro mất dữ liệu khi hỏng hóc phần cứng.

---

## 2. Quy chuẩn Cây thư mục Dự án (kebab-case)
Toàn bộ thư mục và tệp tin trong hệ thống đám mây phải tuân thủ nghiêm ngặt chuẩn **kebab-case** (chữ thường không dấu, dùng dấu gạch ngang `-` để phân tách từ, không dùng khoảng trắng):
- `01-project-overview/` (Tài liệu tổng quan, định hướng dự án)
- `02-architecture-design/` (Sơ đồ kiến trúc hệ thống, thiết kế UI/UX)
- `03-source-code/` (Mã nguồn ứng dụng các phân module)
- `04-meeting-minutes/` (Biên bản họp, ghi chú sprint planning)
- `05-internal-resources/` (Tài liệu hướng dẫn, checklist, SDK công cụ)

---

## 3. Bảng Phân quyền Chia sẻ Google Drive Chuẩn Doanh nghiệp
Để tránh tình trạng rò rỉ dữ liệu hoặc nhầm lẫn quyền chỉnh sửa, việc cấp quyền chia sẻ tệp/thư mục được quy định chặt chẽ như sau:

| Đối tượng nhận quyền | Cấp độ quyền hạn Google Drive | Quy định & Ràng buộc bảo mật |
| :--- | :--- | :--- |
| **Nhân viên mới (Chủ sở hữu)** | **Editor** (Toàn quyền) trên thư mục cá nhân | Quản lý toàn bộ tệp tin trong không gian cá nhân được giao. |
| **Đồng đội cùng dự án** | **Editor** trên thư mục dự án chung | Chỉ cấp quyền trong phạm vi các module/thư mục dự án phụ trách. |
| **Thực tập sinh phòng ban khác** | **Commenter** (Chỉ góp ý) | Chỉ được phép xem và để lại bình luận, **tuyệt đối không** chỉnh sửa trực tiếp nội dung gốc. |
| **Đối tác / Khách mời ngoài** | **Viewer, Restricted** theo Email | **BẮT BUỘC** giới hạn theo địa chỉ email cụ thể. **TUYỆT ĐỐI KHÔNG** dùng chế độ *"Anyone with the link"* đi kèm quyền Editor. |

---

## 4. Văn hóa Giao tiếp Nhóm (Lark / Slack)
- **Sử dụng Channel chuyên biệt:** Các chủ đề trao đổi phải đúng kênh (`#onboarding`, `#dev-frontend`, `#thong-bao-chung`).
- **Reply in Thread:** Luôn sử dụng tính năng trả lời theo chuỗi (Thread) cho từng vấn đề cụ thể để giữ cho kênh chính gọn gàng, không bị trôi tin nhắn.
- **Chống "No-Hello":** Khi cần nhắn tin hỗ trợ, hãy đặt vấn đề trực tiếp kèm ngữ cảnh thay vì chỉ nhắn "Hi", "Alo" rồi chờ đợi người khác phản hồi.
- **Tối giản thông báo:** Hạn chế tối đa việc tag `@all` ngoài giờ làm việc hoặc trong các kênh thông báo chung của công ty.