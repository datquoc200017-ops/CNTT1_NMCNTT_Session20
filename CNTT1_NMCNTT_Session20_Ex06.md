# BÀI TẬP VỀ NHÀ
##   (Bài tập tổng hợp) Hành Trình Xử Lý 1 Lỗi Cài Đặt Thật
### Bài làm
### 1. Lý do câu hỏi "văn nói" (3b) kém hiệu quả
- Chứa nhiều từ thừa, xưng hô không kỹ thuật (`tại sao em`, `vậy thầy ơi`).
- Dùng Tiếng Việt thay vì Tiếng Anh và mã lỗi gốc.
- Thiếu từ khóa môi trường (Windows 11) và thông báo lỗi nguyên văn.

### 2. Bóc tách lỗi (3a)

| Thành phần | Nội dung bóc tách |
| :--- | :--- |
| Tên phần mềm / HDH | Node.js (npm) / Windows 11 |
| Mã lỗi nguyên văn | `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| Thao tác đang làm | Gõ `npm -v` trong Terminal của VS Code |

### 3. 3 câu truy vấn tối ưu (Mỗi câu 1 toán tử)
- `site:`: `site:stackoverflow.com npm is not recognized as an internal or external command windows 11`
- `" "`: `"npm is not recognized as an internal or external command" nodejs windows`
- `-`: `npm is not recognized as an internal or external command windows -xp`

---

## Phần 2 – Thẩm Định StackOverflow

### 1. So sánh Câu trả lời A và B (3c)

| Tiêu chí | Câu trả lời A | Câu trả lời B |
| :--- | :--- | :--- |
| Vote & Tích xanh | +186 Upvotes, Có tích xanh (✓) | +2 Upvotes, Không tích xanh |
| Thời gian đăng | 2 năm trước (mới, phù hợp OS hiện tại) | 9 năm trước** (quá cũ, lỗi thời) |
| Tags khớp | Khớp (`[node.js] [windows]`) | Không khớp (`[windows-xp]`) |

### 2. Kết luận lựa chọn & Bẫy nguy hiểm
- Lựa chọn:  Áp dụng Câu A vì đủ 3 tiêu chí: tích xanh, điểm upvote rất cao, tag khớp Windows hiện tại.
- Bẫy ở Câu B: Gỡ driver mạng của Windows XP không liên quan đến biến PATH trên Windows 11; làm theo dễ gây xung đột hệ thống và hỏng mạng.

### 3. Quy trình 30 Giây Đọc Lướt trên StackOverflow
1. 1–5s: Kiểm tra Tags xem đúng HĐH/công nghệ không.
2. 5–15s: Cuộn ngay xuống câu trả lời có Tích xanh (✓).
3. 15–25s: Soi điểm Upvote (>10) và thời gian đăng bài (gần đây).
4. 25–30s: Đọc lướt đoạn Code/Command trước khi đọc giải thích chi tiết.

###  Prompt 3 Thành phần (Ngữ cảnh – Lỗi – Yêu cầu)

```text
[NGỮ CẢNH]: Tôi vừa cài Node.js trên Windows 11 và mở Terminal VS Code để thực hành. Tôi đã thêm `C:\Program Files\nodejs\` vào PATH và mở lại Terminal mới nhưng vẫn lỗi.

[LỖI NGUYÊN VĂN]:
'npm' is not recognized as an internal or external command, operable program or batch file.

[YÊU CẦU]: Giải thích nguyên nhân vì sao lỗi vẫn còn trong VS Code và đưa ra 2 bước khắc phục bằng Tiếng Việt.
