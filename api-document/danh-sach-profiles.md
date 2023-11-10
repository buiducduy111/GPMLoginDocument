# Danh sách profiles

API URL

```
GET: /api/v3/profiles
```

Params

<table><thead><tr><th width="160">Tên param</th><th width="148">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>group</td><td>Không</td><td>Tên group cần lọc</td></tr><tr><td>page</td><td>Không</td><td>Số trang (mặc định 1)</td></tr><tr><td>per_page</td><td>Không</td><td>Số profile mỗi trang (mặc định 50)</td></tr></tbody></table>

Ví dụ

```
http://127.0.0.1:19995/api/v3/profiles?group=Ebay&page=1&per_page=100
```

Response

```json
[
    {
        "id": "ID_OF_PROFILE",
        "name": "NAME_OF_PROFILE",
        "raw_proxy": "RAW_PROXY",
        "browser_type": "chromium / firefox",
        "browser_version": "BROWSER_VERSISON",
        "group": "NAME_OF_GROUP",
        "profile_path": "Local path or S3",
        "note": "",
        "color": "",
        "created_at": "DATE"
    }
]
```
