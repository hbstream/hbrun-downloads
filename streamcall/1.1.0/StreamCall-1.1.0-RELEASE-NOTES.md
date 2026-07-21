# StreamCall 1.1.0

## English

StreamCall 1.1.0 provides one supported Linux server package and four field endpoint packages.

### Downloads

- `StreamCall-Server-1.1.0-Ubuntu-22.04-x86_64.tar.gz` (ubuntu-22.04-x86_64, linux-tar.gz) - SHA-256 `fb50521b79ad447eee777d62ed0cddbf4cb33a82e5ed3bd3f4a8e62bbfb28084`
- `StreamCall-Endpoint-1.1.0-Windows-x86_64-Setup.exe` (windows-x86_64, windows-installer) - SHA-256 `2df048d4b571a6539c94e7723bad8629f4dcde645daf090bbe851f28d02694ac`
- `StreamCall-Endpoint-1.1.0-Linux-x86_64.AppImage` (linux-x86_64, appimage) - SHA-256 `0c908239920e9b2fb0692b02d5603bec75ee2094975982da160ddfb6752528c7`
- `StreamCall-Endpoint-1.1.0-Android-arm64-v8a.apk` (android-arm64-v8a, apk) - SHA-256 `a369019377bdf1933eec24d89384a8303a268da729dba02f93035d38d7ff7dca`
- `StreamCall-Endpoint-1.1.0-macOS-x86_64.dmg` (macos-x86_64, dmg) - SHA-256 `f10b84938a69c7c97fa4f4e8cb78e4035bb8358cf8837b6d7aab8eeaebcfba24`

### Authorization and platform boundary

- The server package is named StreamCall Server. With no signed license imported, it starts in Free Edition: 1 site, 4 total endpoints including at most 1 dispatcher, 2 linked cameras, and 1 concurrent call, for official first-party clients only.
- Downloading software grants no Starter, Integration, or OEM rights. A 30-day non-commercial evaluation and all commercial or integration rights require separately issued signed authorization; integration also requires app/package identity binding.
- Ubuntu 22.04 x86_64 is the only supported server deployment platform. Windows, Linux, Android, and macOS downloads in the endpoint group cannot be used as servers.
- The Windows installer is not Authenticode-signed. The Android APK is direct-distribution signed but is not an app-store build.
- The macOS DMG is an explicitly labeled direct-download preview. It is ad-hoc signed, not Developer ID signed, not notarized, and has not passed Apple public-distribution gates.
- `public_self_serve_sale_ready=false`: this download channel does not implement self-service paid-license sales.

Verify package hashes against the signed manifest in the official metadata repository. Release public-key SPKI SHA-256: `b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`.

## 简体中文

StreamCall 1.1.0 提供一个受支持的 Linux 服务端包和四个平台的现场终端包。

### 下载文件

- `StreamCall-Server-1.1.0-Ubuntu-22.04-x86_64.tar.gz` (ubuntu-22.04-x86_64, linux-tar.gz) - SHA-256 `fb50521b79ad447eee777d62ed0cddbf4cb33a82e5ed3bd3f4a8e62bbfb28084`
- `StreamCall-Endpoint-1.1.0-Windows-x86_64-Setup.exe` (windows-x86_64, windows-installer) - SHA-256 `2df048d4b571a6539c94e7723bad8629f4dcde645daf090bbe851f28d02694ac`
- `StreamCall-Endpoint-1.1.0-Linux-x86_64.AppImage` (linux-x86_64, appimage) - SHA-256 `0c908239920e9b2fb0692b02d5603bec75ee2094975982da160ddfb6752528c7`
- `StreamCall-Endpoint-1.1.0-Android-arm64-v8a.apk` (android-arm64-v8a, apk) - SHA-256 `a369019377bdf1933eec24d89384a8303a268da729dba02f93035d38d7ff7dca`
- `StreamCall-Endpoint-1.1.0-macOS-x86_64.dmg` (macos-x86_64, dmg) - SHA-256 `f10b84938a69c7c97fa4f4e8cb78e4035bb8358cf8837b6d7aab8eeaebcfba24`

### 授权与平台边界

- 服务端统一命名为 StreamCall Server。未导入签名授权时自动按免费版运行：1 个站点、总计 4 个终端（最多 1 个调度席）、2 路关联摄像头、1 路并发呼叫，并且仅允许官方第一方客户端。
- 下载软件不会授予 Starter、集成或 OEM 权利。30 天非商用评估以及任何商业或集成权利都需要另行签发签名授权；集成授权还要求应用或包身份绑定。
- Ubuntu 22.04 x86_64 是唯一受支持的服务端部署平台。Windows、Linux、Android 和 macOS 终端包均不能作为服务端使用。
- Windows 安装器尚未进行 Authenticode 签名；Android APK 已进行直接分发签名，但不是应用商店构建。
- macOS DMG 明确标记为直接下载预览版：仅临时签名，未使用 Developer ID，未公证，也未通过 Apple 公开发行门禁。
- `public_self_serve_sale_ready=false`：当前下载渠道不包含自助付费授权销售。

请使用官方元数据仓库中的签名清单核对文件。发布公钥 SPKI SHA-256：`b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`。
