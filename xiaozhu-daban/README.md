# 小猪打板公开更新通道

此目录用于“小猪打板”桌面程序的公开稳定版更新清单，不包含私有源码或账号凭据。

- 固定稳定通道：`stable.json`
- 客户端地址：`https://raw.githubusercontent.com/ShaXiaozhu/api/main/xiaozhu-daban/stable.json`
- 后续升级包可放在 GitHub Releases 或公开 Google Drive 文件中。
- 客户端只接受允许列表内的 HTTPS 地址，并校验下载大小、整包 SHA-256 及包内逐文件 SHA-256。

发布新版本的顺序：

1. 通过 `scripts/New-UpdatePackage.ps1` 生成增量升级包与清单数据。
2. 上传升级包并确认公开下载地址可用。
3. 核对升级包大小和 SHA-256。
4. 最后替换 `stable.json`。不要在升级包尚不可下载时提前修改稳定通道清单。

当前 0.3.4 是首个具备软件内升级能力的版本，因此 `package` 为 `null`；后续 0.3.5 及以上版本发布时再填写实际升级包信息。
