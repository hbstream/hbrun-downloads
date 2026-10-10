# HBRun Downloads

[English](#english) | [简体中文](#简体中文)

## English

This repository publishes release notes, checksums, and machine-readable indexes for HBRun product downloads. Installers and SDK archives are distributed through GitHub Releases.

### Current Releases

| Product | Version | Release |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.6.2 | [streamcore-sdk-v1.6.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.6.2) |
| HBRun StreamGate | 1.7.0 | [streamgate-v1.7.0](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.7.0) |
| HBRun StreamCall | Server 1.2.2 / Endpoint 1.2.2 / SDK 1.2.2 | [Current release](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcall-server-v1.2.2-endpoint-v1.2.2) |
| HBRun Connect | 1.2.0 | [hbrun-connect-v1.2.0](https://github.com/hbstream/hbrun-downloads/releases/tag/hbrun-connect-v1.2.0) |

StreamCore SDK demo source and runnable demo packages are published separately in [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo).

StreamCall has ten verified release packages on GitHub. Its [Gitee mirror](https://gitee.com/hbstream/streamcall-downloads/releases/tag/streamcall-server-v1.2.2-endpoint-v1.2.2) carries the nine official-endpoint and SDK packages; the large offline Server archive is GitHub-only. Official applications are Windows EXE/ZIP, Linux x86_64 TGZ, and Android ARM APK. macOS, iOS, Linux aarch64, and Windows Server are not included. StreamCall Server starts in Free Edition when no signed license is imported; downloading a package does not grant commercial API, SDK integration, or OEM rights. Previous releases are retained.

HBRun Connect 1.2.0 currently offers a Linux x86_64 Server package, Windows Expert and attended Field installers/portable packages, and an Android Field APK. The Windows Server packages were withdrawn; integration SDKs and protocol archives are not publicly distributed. The existing Linux Server archive does not include offline recording images, so it is not yet a complete offline Server package. The Windows client executables are intentionally not Authenticode-signed; verify the HTTPS source, size, and SHA-256. The Android APK is release-signed. The current [Gitee mirror](https://gitee.com/hbstream/connect-downloads/releases/tag/hbrun-connect-v1.2.0) carries the same available application assets. Historical release indexes and checksum lists retain withdrawn entries for audit, not as valid download links.

### Official Links

- Website: [https://hbrun.com](https://hbrun.com)
- StreamCore SDK: [https://hbrun.com/products/streamcore-sdk](https://hbrun.com/products/streamcore-sdk)
- StreamGate: [https://hbrun.com/products/streamgate](https://hbrun.com/products/streamgate)
- StreamCall: [https://hbrun.com/products/streamcall](https://hbrun.com/products/streamcall)
- HBRun Connect: [https://hbrun.com/products/hbrun-connect](https://hbrun.com/products/hbrun-connect)
- Downloads: [https://hbrun.com/downloads](https://hbrun.com/downloads)

### Repository Layout

| Directory | Contents |
| --- | --- |
| `manifests/` | Machine-readable latest-release indexes |
| `streamcore-sdk/<version>/` | StreamCore SDK release notes and SHA256 checksums |
| `streamgate/<version>/` | StreamGate release notes and SHA256 checksums |
| `streamcall/<version>/` | StreamCall release notes, authorization boundary, and SHA256 checksums |
| `connect/<version>/` | HBRun Connect release notes, public release index, and SHA256 checksums |

### Verify a Download

Compare the downloaded file with the signed manifest and SHA-256 list in the matching version directory of this metadata repository.

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.7.0-windows-x64-standard-installer.exe
```

## 简体中文

本仓库公开 HBRun 产品下载所需的版本说明、SHA256 校验值和机器可读索引。安装包与 SDK 压缩包通过 GitHub Releases 分发。

### 当前版本

| 产品 | 版本 | 发布页 |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.6.2 | [streamcore-sdk-v1.6.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.6.2) |
| HBRun StreamGate | 1.7.0 | [streamgate-v1.7.0](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.7.0) |
| HBRun StreamCall | 服务端 1.2.2 / 终端 1.2.2 / SDK 1.2.2 | [当前发布](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcall-server-v1.2.2-endpoint-v1.2.2) |
| HBRun Connect | 1.2.0 | [hbrun-connect-v1.2.0](https://github.com/hbstream/hbrun-downloads/releases/tag/hbrun-connect-v1.2.0) |

StreamCore SDK 演示程序源码和可运行演示包在 [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo) 单独发布。

GitHub 提供 StreamCall 本次 10 个已校验交付包；[Gitee 镜像](https://gitee.com/hbstream/streamcall-downloads/releases/tag/streamcall-server-v1.2.2-endpoint-v1.2.2) 提供其中 9 个官方终端与 SDK 包，大型离线服务端包仅通过 GitHub 提供。官方应用为 Windows EXE/ZIP、Linux x86_64 TGZ 与 Android ARM APK；macOS、iOS、Linux aarch64 和 Windows 服务端不属于本次交付。未导入签名授权时服务端按免费版运行；下载不授予商业 API、SDK 集成或 OEM 权利。旧版本保留。

HBRun Connect 1.2.0 当前公开 Linux x86_64 服务端、Windows 专家端和有人值守现场端的安装包/绿色包，以及 Android 现场端 APK。Windows 服务端已撤下；集成 SDK 和协议包暂不公开。现有 Linux 服务端压缩包不含录像离线镜像，尚非完整离线服务包。Windows 客户端按既定决策不做 Authenticode 签名，运行前应核对 HTTPS 来源、文件大小和 SHA-256；Android APK 已做正式发布签名。[Gitee 镜像](https://gitee.com/hbstream/connect-downloads/releases/tag/hbrun-connect-v1.2.0) 提供相同的现存应用附件。历史发行索引及校验清单中的已撤下条目仅供追溯，不再是可用下载链接。

### 官方入口

- 官网：[https://hbrun.com](https://hbrun.com)
- StreamCore SDK：[https://hbrun.com/products/streamcore-sdk](https://hbrun.com/products/streamcore-sdk)
- StreamGate：[https://hbrun.com/products/streamgate](https://hbrun.com/products/streamgate)
- StreamCall：[https://hbrun.com/products/streamcall](https://hbrun.com/products/streamcall)
- HBRun Connect：[https://hbrun.com/products/hbrun-connect](https://hbrun.com/products/hbrun-connect)
- 下载中心：[https://hbrun.com/downloads](https://hbrun.com/downloads)

### 仓库结构

| 目录 | 内容 |
| --- | --- |
| `manifests/` | 最新版本的机器可读索引 |
| `streamcore-sdk/<version>/` | StreamCore SDK 版本说明与 SHA256 校验值 |
| `streamgate/<version>/` | StreamGate 版本说明与 SHA256 校验值 |
| `streamcall/<version>/` | StreamCall 版本说明、授权边界与 SHA256 校验值 |
| `connect/<version>/` | HBRun Connect 版本说明、公开发布索引与 SHA256 校验值 |

### 校验下载文件

下载后请使用本元数据仓库对应版本目录中的签名清单和 SHA-256 列表校验文件完整性。

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.7.0-windows-x64-standard-installer.exe
```
