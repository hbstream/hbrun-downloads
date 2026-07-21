# StreamCall 1.1.0

## English

StreamCall 1.1.0 provides one supported Linux server package and four field endpoint packages.

### Downloads

- `StreamCall-Server-1.1.0-Linux-x86_64.tar.gz` (linux-x86_64, linux-tar.gz) - SHA-256 `9eee87a82a5aa52d3b7fe721edce4ed83ed65013b335adb51ed727c24dde2eeb`
- `StreamCall-Endpoint-1.1.0-Windows-x86_64-Setup.exe` (windows-x86_64, windows-installer) - SHA-256 `2df048d4b571a6539c94e7723bad8629f4dcde645daf090bbe851f28d02694ac`
- `StreamCall-Endpoint-1.1.0-Linux-x86_64.AppImage` (linux-x86_64, appimage) - SHA-256 `dc1ed131005f1259dd8e9324bdf619a7ff3001c0266befeadf3bc4dbb82d9c90`
- `StreamCall-Endpoint-1.1.0-Android-arm64-v8a.apk` (android-arm64-v8a, apk) - SHA-256 `a369019377bdf1933eec24d89384a8303a268da729dba02f93035d38d7ff7dca`
- `StreamCall-Endpoint-1.1.0-macOS-x86_64.dmg` (macos-x86_64, dmg) - SHA-256 `b593d6057a8f4c1d7f870b7b1b034e12eb6cc3f28c440ca05c78cc6238312a92`

### Authorization and platform boundary

- The server package is named StreamCall Server. With no signed license imported, it starts in Free Edition: 1 site, 4 total endpoints including at most 1 dispatcher, 2 linked cameras, and 1 concurrent call, for official first-party clients only.
- Downloading software grants no Starter, Integration, or OEM rights. A 30-day non-commercial evaluation and all commercial or integration rights require separately issued signed authorization; integration also requires app/package identity binding.
- The server tarball targets modern Linux x86_64 without a distribution-name lock. It requires kernel 4.18+, systemd 239+, Python 3.8+, and the packaged host preflight; recording additionally requires Docker Engine 20.10+, FFmpeg/ffprobe 4.4+ with the checked H.264/AAC capabilities, 8 vCPU, and 8 GiB RAM. Ubuntu 22.04 x86_64 remains the full-stack release acceptance baseline. Endpoint downloads cannot be used as servers.
- The Windows installer is not Authenticode-signed. The Android APK is direct-distribution signed but is not an app-store build.
- The macOS DMG is an explicitly labeled direct-download preview. It is ad-hoc signed, not Developer ID signed, not notarized, and has not passed Apple public-distribution gates.
- `public_self_serve_sale_ready=false`: this download channel does not implement self-service paid-license sales.

Verify package hashes against the signed manifest in the official metadata repository. Release public-key SPKI SHA-256: `b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`.

## 简体中文

StreamCall 1.1.0 提供一个受支持的 Linux 服务端包和四个平台的现场终端包。

### 下载文件

- `StreamCall-Server-1.1.0-Linux-x86_64.tar.gz` (linux-x86_64, linux-tar.gz) - SHA-256 `9eee87a82a5aa52d3b7fe721edce4ed83ed65013b335adb51ed727c24dde2eeb`
- `StreamCall-Endpoint-1.1.0-Windows-x86_64-Setup.exe` (windows-x86_64, windows-installer) - SHA-256 `2df048d4b571a6539c94e7723bad8629f4dcde645daf090bbe851f28d02694ac`
- `StreamCall-Endpoint-1.1.0-Linux-x86_64.AppImage` (linux-x86_64, appimage) - SHA-256 `dc1ed131005f1259dd8e9324bdf619a7ff3001c0266befeadf3bc4dbb82d9c90`
- `StreamCall-Endpoint-1.1.0-Android-arm64-v8a.apk` (android-arm64-v8a, apk) - SHA-256 `a369019377bdf1933eec24d89384a8303a268da729dba02f93035d38d7ff7dca`
- `StreamCall-Endpoint-1.1.0-macOS-x86_64.dmg` (macos-x86_64, dmg) - SHA-256 `b593d6057a8f4c1d7f870b7b1b034e12eb6cc3f28c440ca05c78cc6238312a92`

### 授权与平台边界

- 服务端统一命名为 StreamCall Server。未导入签名授权时自动按免费版运行：1 个站点、总计 4 个终端（最多 1 个调度席）、2 路关联摄像头、1 路并发呼叫，并且仅允许官方第一方客户端。
- 下载软件不会授予 Starter、集成或 OEM 权利。30 天非商用评估以及任何商业或集成权利都需要另行签发签名授权；集成授权还要求应用或包身份绑定。
- 服务端压缩包面向现代 Linux x86_64，不锁定发行版名称；要求内核 4.18+、systemd 239+、Python 3.8+ 并通过包内宿主预检。录制还要求 Docker Engine 20.10+、具备已检查 H.264/AAC 能力的 FFmpeg/ffprobe 4.4+、8 vCPU 和 8 GiB 内存。Ubuntu 22.04 x86_64 仍是完整栈发布验收基线。所有终端下载均不能作为服务端使用。
- Windows 安装器尚未进行 Authenticode 签名；Android APK 已进行直接分发签名，但不是应用商店构建。
- macOS DMG 明确标记为直接下载预览版：仅临时签名，未使用 Developer ID，未公证，也未通过 Apple 公开发行门禁。
- `public_self_serve_sale_ready=false`：当前下载渠道不包含自助付费授权销售。

请使用官方元数据仓库中的签名清单核对文件。发布公钥 SPKI SHA-256：`b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`。
