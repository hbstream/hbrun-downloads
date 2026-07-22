# StreamCall 1.1.1

## English

StreamCall 1.1.1 provides one offline Linux server package and four endpoint packages.

### Downloads

- `StreamCall-Server-1.1.1-Linux-x86_64.tar.gz` (linux-x86_64, offline-docker-compose-tar.gz) - SHA-256 `8faa1339cd36e5e32158b98719ae8b19909ff71aeeaaf905f1e82e18a374cb34` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Server-1.1.1-Linux-x86_64.tar.gz) - [Gitee fallback](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Server-1.1.1-Linux-x86_64.tar.gz)
- `StreamCall-Endpoint-1.1.1-Windows-x86_64-Setup.exe` (windows-x86_64, windows-installer) - SHA-256 `0263b5212298168857880cd8c35aa48379956e08db10dbc015970bd1fcf9e0fa` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Windows-x86_64-Setup.exe) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Windows-x86_64-Setup.exe)
- `StreamCall-Endpoint-1.1.1-Linux-x86_64.AppImage` (linux-x86_64, appimage) - SHA-256 `d5e4cf4206863d1f0775528edc4943b05204efb9526b6f7aadfdcc5980be4a0a` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Linux-x86_64.AppImage) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Linux-x86_64.AppImage)
- `StreamCall-Endpoint-1.1.1-Android-arm64-v8a.apk` (android-arm64-v8a, apk) - SHA-256 `d2036d98f526e8f6fdb2f05a23977cd3f557c530b2870a40f9cbf31c88eadf37` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Android-arm64-v8a.apk) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Android-arm64-v8a.apk)
- `StreamCall-Endpoint-1.1.1-macOS-x86_64.dmg` (macos-x86_64, dmg) - SHA-256 `4e953d2a2913aafd4cc2e42273b9b5204f2ef8c699e870fd336024a778f3df64` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-macOS-x86_64.dmg) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-macOS-x86_64.dmg)

### Deployment and authorization

- The Linux server is one offline Docker Compose package. It carries five exact container images, including FFmpeg/ffprobe in the StreamCall image; the buyer host does not install StreamCall, Nginx, Redis, LiveKit, Egress, FFmpeg, or ffprobe packages separately and does not need registry access during installation.
- Supported hosts are modern Linux x86_64 systems that pass the packaged preflight: kernel 4.18+, rootful Docker Engine 20.10+, Compose v2.24+, 8 logical CPUs, 7.5 GiB memory, 12 GiB free disk, and an accepted Docker storage driver. Ubuntu 22.04 is the full-stack acceptance baseline; Debian 12 and Rocky Linux 9 are host-contract compatibility baselines.
- Without a signed license the server runs in Free Edition: 1 site, 4 total endpoints including at most 1 dispatcher, 2 linked cameras, and 1 concurrent call, for official first-party clients only.
- Downloading software grants no Starter, Integration, API/SDK, or OEM rights. A 30-day non-commercial evaluation and all commercial or integration rights require a separately issued signed authorization. Integration authorization also requires application or package identity binding.
- Endpoint packages cannot be deployed as servers. The Windows installer is not Authenticode-signed. The Android APK is signed for direct distribution but is not an app-store build.
- The macOS DMG is a direct-download preview: it is ad-hoc signed, not Developer ID signed, not notarized, and does not claim Apple public-distribution readiness.
- GitHub hosts all five exact packages. Gitee natively mirrors the four endpoint packages. Its 100 MiB per-attachment limit cannot carry the 1.63 GB offline server archive, so the Gitee release links the same exact GitHub server asset instead of splitting or repacking it.
- `public_self_serve_sale_ready=false`: licensing remains assisted-sale rather than self-service checkout.

Verify every download against the signed manifest. Release public-key SPKI SHA-256: `b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`.

## 简体中文

StreamCall 1.1.1 提供一个离线 Linux 服务端包和四个终端安装包。

### 下载文件

- `StreamCall-Server-1.1.1-Linux-x86_64.tar.gz` (linux-x86_64, offline-docker-compose-tar.gz) - SHA-256 `8faa1339cd36e5e32158b98719ae8b19909ff71aeeaaf905f1e82e18a374cb34` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Server-1.1.1-Linux-x86_64.tar.gz) - [Gitee fallback](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Server-1.1.1-Linux-x86_64.tar.gz)
- `StreamCall-Endpoint-1.1.1-Windows-x86_64-Setup.exe` (windows-x86_64, windows-installer) - SHA-256 `0263b5212298168857880cd8c35aa48379956e08db10dbc015970bd1fcf9e0fa` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Windows-x86_64-Setup.exe) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Windows-x86_64-Setup.exe)
- `StreamCall-Endpoint-1.1.1-Linux-x86_64.AppImage` (linux-x86_64, appimage) - SHA-256 `d5e4cf4206863d1f0775528edc4943b05204efb9526b6f7aadfdcc5980be4a0a` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Linux-x86_64.AppImage) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Linux-x86_64.AppImage)
- `StreamCall-Endpoint-1.1.1-Android-arm64-v8a.apk` (android-arm64-v8a, apk) - SHA-256 `d2036d98f526e8f6fdb2f05a23977cd3f557c530b2870a40f9cbf31c88eadf37` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Android-arm64-v8a.apk) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-Android-arm64-v8a.apk)
- `StreamCall-Endpoint-1.1.1-macOS-x86_64.dmg` (macos-x86_64, dmg) - SHA-256 `4e953d2a2913aafd4cc2e42273b9b5204f2ef8c699e870fd336024a778f3df64` - [GitHub](https://github.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-macOS-x86_64.dmg) - [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases/download/streamcall-v1.1.1/StreamCall-Endpoint-1.1.1-macOS-x86_64.dmg)

### 部署与授权边界

- Linux 服务端采用单一离线 Docker Compose 包，内含五个精确容器镜像。FFmpeg/ffprobe 已位于 StreamCall 镜像内；客户宿主无需分别安装 StreamCall、Nginx、Redis、LiveKit、Egress、FFmpeg 或 ffprobe，安装过程也不需要访问镜像仓库。
- 支持通过包内预检的现代 Linux x86_64 宿主：内核 4.18+、rootful Docker Engine 20.10+、Compose v2.24+、8 个逻辑 CPU、7.5 GiB 内存、12 GiB 可用磁盘及受支持的 Docker 存储驱动。Ubuntu 22.04 是完整栈验收基线；Debian 12 和 Rocky Linux 9 是宿主合同兼容性基线。
- 未导入签名授权时，服务端按 Free Edition 运行：1 个站点、总计 4 个终端（最多 1 个调度席）、2 路关联摄像头、1 路并发呼叫，并且仅允许官方第一方客户端。
- 下载软件不会授予 Starter、集成、API/SDK 或 OEM 权利。30 天非商用评估及所有商业或集成权利都需要另行签发的签名授权；集成授权还要求绑定应用或包身份。
- 终端安装包不能作为服务端部署。Windows 安装器尚未进行 Authenticode 签名；Android APK 已完成直接分发签名，但不是应用商店构建。
- macOS DMG 是直接下载预览包：仅临时签名，未使用 Developer ID，未公证，也不声称已满足 Apple 公开分发要求。
- GitHub 托管全部五个精确软件包。Gitee 原生镜像四个终端包；由于其单附件 100 MiB 限制无法容纳 1.63 GB 离线服务端包，Gitee 发布页会链接同一个 GitHub 精确服务端包，不拆分也不重新打包。
- `public_self_serve_sale_ready=false`：当前仍采用人工协助授权销售，不包含自助结算。

请使用签名清单核对全部下载文件。发布公钥 SPKI SHA-256：`b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`。
