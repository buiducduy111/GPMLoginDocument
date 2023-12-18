# Mở profile

API URL

```
GET: /api/v3/profiles/start/{id}
```

Params:

| Tên param        | Bắt buộc | Mô tả                                                                                         |
| ---------------- | -------- | --------------------------------------------------------------------------------------------- |
| addination\_args | Không    | Các param khởi động cùng trình duyệt, cần hiểu rõ về trình duyệt mới có thể dùng thông số này |
| win\_scale       | Không    | Giá trị từ 0 tới 1.0                                                                          |
| win\_pos         | Không    | Giá trị tọa độ trình duyệt theo dạng x,y                                                      |
| win\_size        | Không    | Giá trị width,height                                                                          |

Ví dụ

```
http://127.0.0.1:19995/api/v3/profiles/open/id=xgyasg1995?win_scale=0.8&win_pos=300,300    
```

Repsonse

```json
{
    "success": true,
    "message": "Khởi tạo thành công",
    "profile_id": "ID_OF_PROFILE",
    "browser_path": "PATH of browser",
    "driver_path": "PATH of driver",
    "remote_debugging_port": REMOTE_PORT
}
```
