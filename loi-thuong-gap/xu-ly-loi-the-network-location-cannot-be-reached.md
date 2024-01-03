---
description: Lỗi xuất hiện ngay khi mở ứng dụng
---

# Xử lý lỗi: The network location cannot be reached

* Cách khắc phục: Mở cmd với quyền admin (cmd nha không phải powershell) và chạy lệnh: **netsh http add iplisten 127.0.0.1** hoặc **sc config http start=demand**
* Nguyên nhân: Do tool khởi tạo một HttpServer tại địa chỉ 127.0.0.1 để phục vụ việc export cookie, nhưng máy chưa cho phép lắng nghe dữ liệu tại địa chỉ này nên lỗi

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
