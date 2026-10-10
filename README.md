# Release

Bản phát hành các ứng dụng của ELGLabs. File APK và IPA nằm ở mục
[Releases](https://github.com/ELGLabs/Release/releases), tên theo dạng
`<TênApp>-<tag>`, ví dụ `OnlineDLU-v1.3.0.apk`.

## Cài ứng dụng iOS

IPA phát hành **chưa ký**. Thêm nguồn ELGLabs vào LiveContainer, AltStore hoặc
SideStore để cài và nhận cập nhật; trình cài sẽ tự ký bằng Apple ID của bạn.

```
https://app.elglabs.org/ios.json
```

- **LiveContainer:** Sources → nút **+** → dán link trên.
- **AltStore / SideStore:** Browse → Sources → nút **+** → dán link trên.

Không dùng nguồn thì tải thẳng file `.ipa` ở Releases rồi ký bằng Sideloadly.

## Ứng dụng

| App | Android | iOS |
|---|---|---|
| [Online DLU](https://app.elglabs.org/app/org.elglabs.dluonline) | `OnlineDLU-<tag>.apk` | `OnlineDLU-<tag>.ipa` (có trong `ios.json`) |

Ảnh đại diện và ảnh màn hình của từng app nằm trong `assets/<App>/`.

## Thêm bản mới vào ios.json

Mỗi bản phát hành iOS là một mục mới **ở đầu** mảng `versions` của app, kèm
`size` đúng bằng số byte của file IPA trên Releases. Cập nhật luôn các trường
cũ `version`, `versionDate`, `versionDescription`, `downloadURL`, `size` ở cấp
app cho các bản AltStore / LiveContainer đời trước.
