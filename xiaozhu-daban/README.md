# 小猪打板公开更新通道

此目录仅用于“小猪打板”桌面程序的公开稳定版更新清单。

- 稳定通道清单：`updates/stable.json`
- 安装包：GitHub Releases，标签格式 `xiaozhu-daban-v<版本号>`
- 客户端只接受公开 HTTPS 地址，并校验安装包 SHA-256、大小及包内逐文件哈希清单。

发布顺序：先上传并验证 Release 安装包，最后更新 `updates/stable.json`。不要在安装包尚不可下载时提前修改稳定通道清单。
