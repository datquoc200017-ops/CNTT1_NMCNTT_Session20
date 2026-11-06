# BÀI TẬP VỀ NHÀ
##  Bài 3 : Ứng dụng mô hình IPO trong xử lý lỗi Git
### Bài làm


**3. Yêu cầu đầu ra**

**_Báo cáo phân tích (IPO)_**

1.   Xác định Input (Ngữ cảnh + Mã lỗi nguyên văn), Process (Cách AI xử lý thông tin), Output (Bản dịch và 3 bước sửa lỗi).
- Input ngữ cảnh bạn gõ lệnh git và gặp mã lỗi bài là **"fatal: not a git repository (or any of the parent directories): .git"** Process: Từ cách bạn đó viết và đưa vào chatgpt hoặc gemini AI sẽ xử lý dòng lệnh và đưa ra câu trả lời chuẩn xác nhất.
- 3 bước xử lý

3 bước xử lý lỗi `fatal: not a git repository`:

1.  Kiểm tra thư mục hiện tại:
    
    ```
    pwd
    ```
    
2.  Di chuyển vào thư mục dự án:
    
    ```
    cd đường_dẫn_thư_mục_dự_án
    ```
    
3.  Khởi tạo Git và kiểm tra:
    
    ```
    git init
    git status
    ```
    

Kết quả

Git đã được khởi tạo và có thể sử dụng các lệnh Git trong dự án.

    
1.   Viết câu Prompt hoàn chỉnh theo đúng công thức: Ngữ cảnh → Mã lỗi → Yêu cầu.
- **NGỮ CẢNH:**

Tôi đang sử dụng Git để quản lý mã nguồn dự án lập trình. Khi thực hiện lệnh Git trong Terminal, hệ thống không nhận diện được repository hiện tại.

**MÃ LỖI:**

```
fatal: not a git repository (or any of the parent directories): .git
```

**YÊU CẦU:

Hãy hướng dẫn tôi xử lý lỗi trên theo đúng 3 bước:

1.  Kiểm tra vị trí thư mục hiện tại bằng lệnh `pwd`.
    
2.  Di chuyển đến đúng thư mục dự án bằng lệnh `cd`.
    
3.  Kiểm tra Git bằng `git status`; nếu dự án chưa được khởi tạo Git thì sử dụng `git init`.
    
    

