### Bước 1: Phân tích lỗi của prompt cũ

Khi chạy prompt gốc (_"Hãy giải thích ngắn gọn các nội dung của Custom Instructions, Prompt Library, Prompt Injection"_), AI thường tự động chèn thêm 3 phần văn bản thừa thãi gây tốn thời gian cắt gọt khi dán vào báo cáo:

1.  **Câu chào hỏi và xác nhận yêu cầu (Mở đầu xã giao):** Ví dụ:  _"Chào bạn! Dưới đây là phần giải thích ngắn gọn về ba khái niệm bạn đang quan tâm..."_
    
2.  **Đoạn dẫn nhập tổng quan hoặc chuyển ý (Đệm thông tin):** Ví dụ:  _"Trong lĩnh vực quản trị AI, việc nắm vững các thuật ngữ này rất quan trọng. Cụ thể như sau:"_
    
3.  **Lời kết thúc và gợi ý mở rộng (Đuôi xã giao):** Ví dụ:  _"Hy vọng những thông tin trên hữu ích cho bạn. Nếu bạn muốn tìm hiểu sâu hơn về cách phòng chống Prompt Injection, hãy cho tôi biết nhé!"_
    

### Bước 2: Viết prompt tối ưu

Để ép AI chỉ xuất ra dữ liệu thô, sạch chữ thừa và đúng chuẩn báo cáo, bạn sử dụng cấu trúc ràng buộc (Constraints) sau:

> **Prompt tối ưu:** Giải thích định nghĩa và vai trò của 3 khái niệm: Custom Instructions, Prompt Library, Prompt Injection.
> 
> **Ràng buộc định dạng bắt buộc:**
> 
> -   Trình bày bằng danh sách gạch đầu dòng (`-`), in đậm tên từng khái niệm.
>     
> -   Mỗi khái niệm giải thích tối đa 2 câu, đi thẳng vào bản chất kỹ thuật.
>     
> -   **TUYỆT ĐỐI KHÔNG** viết lời chào mở đầu, câu dẫn nhập, câu chuyển ý hay lời kết xã giao. Bắt đầu ngay bằng gạch đầu dòng đầu tiên.
>     

### Kết quả phản hồi của AI (Khi áp dụng prompt tối ưu)

-   **Custom Instructions:** Là tính năng cho phép người dùng thiết lập sẵn ngữ cảnh, vai trò và quy tắc phản hồi cố định cho AI. Công cụ này giúp duy trì sự nhất quán trong mọi cuộc hội thoại mà không cần lặp lại yêu cầu ban đầu.
    
-   **Prompt Library:** Là kho lưu trữ các mẫu câu lệnh (prompt) đã được chuẩn hóa và tối ưu theo từng tác vụ cụ thể. Hệ thống này giúp tăng tốc độ làm việc, đảm bảo chất lượng đầu ra đồng đều và dễ dàng chia sẻ trong đội nhóm.
    
-   **Prompt Injection:** Là kỹ thuật tấn công bảo mật bằng cách chèn các câu lệnh độc hại ngụy trang vào dữ liệu đầu vào. Mục đích của hành vi này là đánh lừa AI bỏ qua các quy tắc an toàn gốc để tiết lộ thông tin nhạy cảm hoặc thực thi hành vi trái phép.
