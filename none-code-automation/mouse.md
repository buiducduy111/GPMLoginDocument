# Mouse

Chức năng các action

<table><thead><tr><th width="223">Action</th><th>Mô tả</th></tr></thead><tbody><tr><td>Mouse move</td><td>Di chuyển chuột vào một element</td></tr><tr><td>Mouse click</td><td>Click chuột vào một element</td></tr><tr><td>Mouse try to click</td><td>Click chuột nhiều lần vào một element tới khi thỏa mãn điều kiện</td></tr></tbody></table>

<mark style="color:red;">**Chú ý: tất cả các đầu vào đều có thể nhúng các biến khác bằng định dạng $TÊN\_BIẾN**</mark>

**Mouse click**

* Đầu vào: Xpath, Element index : trong trường hợp xpath xác định được nhiều element, element index giúp chọn chính xác vào element cần thao tác theo index (tính từ 0)

**Mouse try to click**

* Đầu vào: Xpath, Tham số điều kiện click

Tham số điều kiện click bao gồm:

1. Try count : số lần thử click tối đa
2. Delay each try: thời gian chờ mỗi lần click (tính bằng giây)
3. Điều kiện dừng (xem tại mục menu block, điều kiện tương tự sử dụng cho các khối  if, while)

Phần mềm sẽ click liên tục tới khi một trong 2 điều kiện (Try count hoặc điều kiện dừng) được thỏa mãn.
