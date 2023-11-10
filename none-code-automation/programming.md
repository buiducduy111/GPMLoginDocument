# Programming

**Chức năng các action**

Chi tiết sử dụng từng action xem bên dưới.

<table data-full-width="false"><thead><tr><th width="269">Action</th><th>Mô tả</th></tr></thead><tbody><tr><td>Declare variable</td><td>Khai báo một biến</td></tr><tr><td>Random number</td><td>Tạo một số ngẫu nhiên</td></tr><tr><td>Split text</td><td>Cắt chuỗi thành một mảng kí tự</td></tr><tr><td>Math execute</td><td>Thực hiện một chuỗi phép toán</td></tr><tr><td>Read random line</td><td>Đọc dòng ngẫu nhiên ở một file txt</td></tr><tr><td>Delay</td><td>Dừng chờ</td></tr><tr><td>Http Get</td><td>Thực hiện request GET</td></tr><tr><td>Http Post</td><td>Thực hiện request POST</td></tr><tr><td>Http Download</td><td>Thực hiện request DOWNLOAD</td></tr><tr><td>Read Json</td><td>Đọc một node của json</td></tr><tr><td>Break loop</td><td>Thoát vòng lặp</td></tr><tr><td>Create excel workbook</td><td>Tạo file excel</td></tr><tr><td>Export excel</td><td>Ghi excel</td></tr><tr><td>Get clipboard</td><td>Lấy đoạn text đang lưu trong bộ nhớ</td></tr><tr><td>Set clipboard</td><td>Set text vào trong bộ nhớ</td></tr></tbody></table>

<mark style="color:red;">**Chú ý: tất cả các đầu vào đều có thể nhúng các biến khác bằng định dạng $TÊN\_BIẾN**</mark>



**Declare variable**

* Đầu vào: Giá trị cần đưa vào (có thể nhúng biến khác thông qua kí tự $, ví dụ $giatri1)
* Đầu ra: tên biến lưu kết quả

**Random number**

* Đầu vào: Khoảng giá trị cần random. Ví dụ : 10,20 (cho phép nhúng biến, ví dụ: $min, $max)
* Đầu ra: tên biến lưu kết quả

**Split text**

* Đầu vào: chuỗi có định dạng

```
Text;Kí tự phân cách
```

Ví dụ

```
buiducduygame1@gmail.com|MyPassword@123;|

--> Phân cách chuỗi buiducduygame1@gmail.com|MyPassword@123 bởi kí tự |
```

* Đầu ra: tên biến lưu kết quả

```
Biến này có định dạng mảng nên có thể truy cập như sau
$test[0], $test[1], $test[2]...
Trong ví dụ trên, nếu điền biến đầu ra là test thì ta có

$test[0] - buiducduygame1@gmail.com
$test[1] - MyPassword@123

```

**Math execute**

* Đầu vào: một chuỗi các phép toán cần thực hiện

```
Ví dụ:
$giaTri1 + 10 - 5*2
```

* Đầu ra: tên biến lưu kết quả

**Read random line**

* Đầu vào: đường dẫn tới file text trong máy
* Đầu ra: tên biến lưu kết quả

**Delay**

* Đầu vào: khoảng thời gian cần dely theo định dạng min,max tính theo milisecond (ví dụ: 1000,3000 --> từ 1 tới 3 giây)

**Http Get**

* Đầu vào: Get URL
* Đầu ra: tên biến lưu kết quả

**Http Post**

* Đầu vào: định dạng URL;Data

\+ Post URL

\+ Data : dạng raw, có thể là json hoặc dạng nối param như email=buiducduygame@gmail.com\&password=Abc1234, tùy thuộc vào quy định của api cần gọi

```
Ví dụ:
https://api.gpmloginapp.com/profiles/create;{"name": "Test profile"}
```

* Đầu ra: tên biến lưu kết quả

**Http Download**

* Đầu vào: định dạng URL;Đường dẫn cần lưu trên máy

**Read Json**

* Đầu vào: định dạng Json;node 1;node 2;node 3....

```
Ví dụ có một json như sau được lưu vào biến $ketQua

{
    "name": "Test profile",
    "info": {
        "created_at": "2023-11-11",
        "author": "buiducduygame"
    }
}

Để đọc được author dùng như sau:
$ketQua;info;author
```

* Đầu ra: tên biến lưu kết quả

**Create excel workbook**

* Đầu vào: đường dẫn cần lưu file excel nếu chạy lệnh export
* Đầu ra: tên biến lưu kết quả, excel tạm sẽ lưu trong bộ nhớ

**Export excel**

* Đầu vào: định dạng $tên\_biến\_create\_excel\_workbook;Tên cột;Dữ liệu

Dòng excel sẽ được sinh tự động một cách tuần tự, ví dụ cột A1 đã có dữ liệu, phần mềm sẽ tự động ghi vào cột A2

**Get clipboard**

* Đầu ra: tên biến lưu kết quả

**Set clipboard**

* Đầu vào: giá trị text cần set
