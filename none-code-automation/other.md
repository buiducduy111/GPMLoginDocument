# Other

Chức năng các action

<table><thead><tr><th width="223">Action</th><th>Mô tả</th></tr></thead><tbody><tr><td>Switch to popup</td><td>Đổi trình điều khiển sang một popup theo title</td></tr><tr><td>Swtich to frame</td><td>Đổi trình điều khiển sang một frame</td></tr><tr><td>Switch to default</td><td>Đổi trình điều khiển về cửa sổ mặc định</td></tr><tr><td>Accept alert</td><td>Nhấn đồng ý một alert</td></tr><tr><td>Cancel alert</td><td>Nhấn hủy bỏ một alert</td></tr><tr><td>Execute javascript</td><td>Chạy một đoạn mã javascript</td></tr><tr><td>Import cookie</td><td>Import cookie từ file json</td></tr><tr><td>Export cookie</td><td>Export cookie ra file son</td></tr></tbody></table>

<mark style="color:red;">**Chú ý: tất cả các đầu vào đều có thể nhúng các biến khác bằng định dạng $TÊN\_BIẾN**</mark>

**Switch to popup**

Đầu vào: đoạn text chứa trong title của popup

**Execute javascript**

Đây lầ một action rất mạnh, cho phép tính toán và thực hiện những công việc app chưa hỗ trợ, javascript cũng giúp thực hiện đa số automation trên một website

Đầu vào có thể là một đoạn javascript (cần dùng các công cụ online để convert nhiều dòng thành một dòng) hoặc đường dẫn tới file javascript (trường hợp code quá dài)

Chú ý: nếu lưu đầu ra cho action, cần sử dụng **return** trong code js.
