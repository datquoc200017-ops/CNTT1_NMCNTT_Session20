# BÀI TẬP VỀ NHÀ
##   Bài 4 : Đánh giá công cụ hỗ trợ xử lý lỗi lập trình
### Bài làm
### Bảng So Sánh

| Tiêu chí | Phương án 1: Cảm tính / Nhóm Chat | Phương án 2: Quy trình 4 Chặng Chuẩn hóa |
| :--- | :--- | :--- |
| Downtime (Thời gian chết) | Kéo dài — Phụ thuộc vào thời gian rảnh của Senior Dev. | Rút ngắn 80% — Tự xử lý tại chỗ trong 5–15 phút. |
| Áp lực & Chi phí Senior | Rất cao — Bị phân tâm liên tục bởi các lỗi lặp lại. | Tối ưu — Senior chỉ nhận ca khó đã có Bug Report. |
| Năng lực & Tự chủ KTV | Thụ động — Sợ lỗi tiếng Anh, không tiến bộ. | Chủ động — Tư duy phân tích tốt, tự chủ vận hành. |
| Lưu vết tri thức | Thất thoát — Tin nhắn bị trôi trên Zalo/Telegram. | Tích lũy tập trung — Tạo nguồn tài liệu Wiki nội bộ. |

> Kết luận cho Ban Giám đốc: Bắt buộc chọn Phương án 2 khi nâng quy mô lên 1,000 trạm sạc nhằm:
> 1. Cắt giảm thiệt hại: Tránh bùng nổ chi phí Downtime (500,000 VNĐ/giờ/trụ).
> 2. Giải tỏa nguồn lực: Loại bỏ nút thắt cổ chai ở đội ngũ Senior Dev.
> 3. Đóng gói quy trình: Dễ dàng chuẩn hóa và đào tạo KTV mới trên toàn quốc.

---

## 2. Sơ Đồ Luồng Ra Quyết Định Gỡ Lỗi (Decision Flowchart)

```text
[MÀN HÌNH KIOSK BÁO LỖI]
         │
         ▼
[CHẶNG 1: Google Toán tử]
(Bóc tách mã lỗi ➔ Tìm kiếm với toán tử site:, "", -)
         │
         ├─► Tìm thấy cách sửa? ──► [Thực thi ➔ Thành công]
         │
         ▼ (Chưa xong)
[CHẶNG 2: StackOverflow / GitHub]
(Đọc lướt 30s ➔ Chọn câu trả lời có Tích xanh ✓ / Upvote cao)
         │
         ├─► Tìm thấy giải pháp? ─► [Thực thi ➔ Thành công]
         │
         ▼ (Chưa xong)
[CHẶNG 3: Hỏi Trợ lý AI]
(Gửi Prompt 3 thành phần ➔ Thử tối đa 2 giải pháp của AI)
         │
         ├─► Sửa được lỗi? ───────► [Thành công]
         │
         ▼ (Nếu thất bại sau 15 phút)
[CHẶNG 4: Lập phiếu Bug Report]
(Đóng gói thông tin theo chuẩn 4 bước ➔ Chuyển lên IT Helpdesk / Senior Dev)
