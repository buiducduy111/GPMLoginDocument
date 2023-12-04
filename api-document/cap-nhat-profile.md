# Cập nhật profile

API URL

```
POST /api/v3/profiles/update/{profile_id}
```

Post data

```json
{
    "profile_name" : "NAME_OF_PROFILE",
    "group_id": 1,
    "raw_proxy" : "",
    "startup_urls": "",
    "note": "",
    "color": "COLOR_HEX",
    "user_agent": "auto"
}
```

Giải thích các thông số:

<table><thead><tr><th width="224">Tên trường</th><th width="134">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>name</td><td>Có</td><td>Tên của profile</td></tr><tr><td>group</td><td>Không</td><td>Tên của group</td></tr><tr><td>raw_proxy</td><td>Không</td><td>HTTP proxy| IP:Port:User:Pass<br>Socks5| socks5://IP:Port:User:Pass<br>TMProxy| tm://API_KEY|True,False<br>TinProxy| tin://API_KEY|True,False<br>TinsoftProxy| tinsoft://API_KEY|True,False</td></tr><tr><td>startup_urls</td><td>Không</td><td>Url 1, Url 2, Url 3</td></tr><tr><td>note</td><td>không</td><td>Ghi chú</td></tr><tr><td>color</td><td>Không</td><td>Mã hex màu profile</td></tr><tr><td>user_agent</td><td>Không</td><td>"auto" hoặc tự điền</td></tr></tbody></table>

Reponse

```json
{
    "success": true
}
```
