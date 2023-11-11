# Helper

Chức năng các action

<table><thead><tr><th width="223">Action</th><th>Mô tả</th></tr></thead><tbody><tr><td>Read mail code</td><td>Đọc email code</td></tr></tbody></table>

<mark style="color:red;">**Chú ý: tất cả các đầu vào đều có thể nhúng các biến khác bằng định dạng $TÊN\_BIẾN**</mark>

**Read mail code**

Chú ý: mail phải được bật IMAP để sử dụng tính năng này, thông thường chỉ đối với gmail, tính năng này cần bật thủ công, còn lại các mail khác đều đã bật sẵn khi tạo tài khoản. Áp dụng tốt cho outlook.

* Đầu vào:

1. Sender contains: đoạn text chứa trong email của người gửi (ví dụ email của ebay là no-reply@ebay.com)
2. Code len or xpath: độ dài của code cần đọc (thông thường là 6 số) - nếu trong trường hợp code về dạng số hoặc xpath - nếu trường hợp code về dạng chữ (cần dùng xpath để lọc ra code đó trong html)
3. User: tài khoản mail
4. Pass: mật khẩu email
5. Mail server: cho biết loại mail là gì, search google theo từ khóa: imap server of XXX (ví dụ : imap server of outlook là outlook.office365.com, của gmail là imap.gmail.com)
6. Xpath atrr: trong trường hợp code về là chữ, cần lọc bằng xpath (ở bước số 2) thì cần điền thêm attribute để cho app biết sẽ lấy ở đâu.
