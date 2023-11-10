# Tạo profile

API URL

```
POST /api/v3/profiles/create
```

Post data

```json
{
    "name" : "NAME_OF_PROFILE",
    "group": "NAME_OF_GROUP",
    "browser_core": "chromium",
    "browser_version": "newest",
    "raw_proxy" : "",
    "startup_urls": "",
    "fingerprint" :
    {
        "os": "Windows 11",
        "os_platform": "64bit",
        "timezone": "auto",
        "geolocation": "auto",
        "webrtc": "auto",
        "screen": "1366x768",
        "canvas": "real",
        "client_rect": "real",
        "webgl": "real",
        "webgl_meta": "auto",
        "audio": "noise",
        "font": "auto",
        "user_agent": "auto"
    }
}
```

Giải thích các thông số:

<table><thead><tr><th width="224">Tên trường</th><th width="134">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>name</td><td>Có</td><td>Tên của profile</td></tr><tr><td>group</td><td>Không</td><td>Tên của group</td></tr><tr><td>browser_core</td><td></td><td>chromium, firefox</td></tr><tr><td>browser_version</td><td></td><td>"auto" hoặc tự điền</td></tr><tr><td>raw_proxy</td><td></td><td>HTTP proxy| IP:Port:User:Pass<br>Socks5| socks5://IP:Port:User:Pass<br>TMProxy| tm://API_KEY|True,False<br>TinProxy| tin://API_KEY|True,False<br>TinsoftProxy| tinsoft://API_KEY|True,False</td></tr><tr><td>startup_urls</td><td></td><td>Url 1, Url 2, Url 3</td></tr><tr><td>fingerprint.os</td><td></td><td>"auto" hoặc tự điền</td></tr><tr><td>fingerprint.os_platform</td><td></td><td>"auto" hoặc tự điền</td></tr><tr><td>fingerprint.timezone</td><td></td><td>"auto" hoặc tự điền</td></tr><tr><td>fingerprint.geolocation</td><td></td><td>auto, off</td></tr><tr><td>fingerprint.webrtc</td><td></td><td>auto, off hoặc điền fixed IP</td></tr><tr><td>fingerprint.screen</td><td></td><td>"auto" hoặc tự điền</td></tr><tr><td>fingerprint.canvas</td><td></td><td>real, noise</td></tr><tr><td>fingerprint.webgl</td><td></td><td>real, noise</td></tr><tr><td>fingerprint.webgl_meta</td><td></td><td>auto, real</td></tr><tr><td>fingerprint.audio</td><td></td><td>real, noise</td></tr><tr><td>fingerprint.font</td><td></td><td>auto, off</td></tr><tr><td>fingerprint.useragent</td><td></td><td>"auto" hoặc tự điền</td></tr></tbody></table>

Reponse

```json
{
    "success": true,
    "id": "PROFILE_ID",
    "name": "PROFILE_NAME",
    "path": "PROFILE_LOCAL_PATH or S3_PATH",
    "group": "NAME_OF_GROUP",
    "browser_type": "chromium or firefox",
    "browser_version": "VERSION"
}
```
