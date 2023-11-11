# Element

Chức năng các action

<table><thead><tr><th width="223">Action</th><th>Mô tả</th></tr></thead><tbody><tr><td>Wait element</td><td>Chờ element xuất hiện</td></tr><tr><td>Get element text</td><td>Lấy text cả element</td></tr><tr><td>Get element attribute</td><td>Lấy dữ liệu trong attribute của element</td></tr><tr><td>Count element</td><td>Điếm số lượng element theo xpath</td></tr></tbody></table>

<mark style="color:red;">**Chú ý: tất cả các đầu vào đều có thể nhúng các biến khác bằng định dạng $TÊN\_BIẾN**</mark>

**Wait element**

* Đầu vào: Xpath, Wait time in seconds : thời gian chờ tối đa tính bằng giây, nếu quá thời gian này sẽ coi là có lỗi xảy ra

**Get element attribute**

* Đầu vào: Xpath, tên attribute cần lấy

```
Ví dụ

<a id="linkBtn" href="https://gpmloginapp.com">Click để tới trang chủ</a>

XPATH = //a[@id='linkBtn']
ATTRIBUTE = href

--> Kết quả trả ra: https://gpmloginapp.com
```

* Đầu ra: tên biến lưu kết quả
