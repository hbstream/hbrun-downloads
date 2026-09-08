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

StreamCore SDK demo source and runnable demo packages are published separately in [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo).

StreamCall has ten verified release packages on GitHub. Its [Gitee mirror](https://gitee.com/hbstream/streamcall-downloads/releases/tag/streamcall-server-v1.2.2-endpoint-v1.2.2) carries the nine official-endpoint and SDK packages; the large offline Server archive is GitHub-only. Official applications are Windows EXE/ZIP, Linux x86_64 TGZ, and Android ARM APK. macOS, iOS, Linux aarch64, and Windows Server are not included. StreamCall Server starts in Free Edition when no signed license is imported; downloading a package does not grant commercial API, SDK integration, or OEM rights. Previous releases are retained.

### Official Links

- Website: [https://hbrun.com](https://hbrun.com)
- StreamCore SDK: [https://hbrun.com/products/streamcore-sdk](https://hbrun.com/products/streamcore-sdk)
- StreamGate: [https://hbrun.com/products/streamgate](https://hbrun.com/products/streamgate)
- StreamCall: [https://hbrun.com/products/streamcall](https://hbrun.com/products/streamcall)
- Downloads: [https://hbrun.com/downloads](https://hbrun.com/downloads)

### Repository Layout

| Directory | Contents |
| --- | --- |
| `manifests/` | Machine-readable latest-release indexes |
| `streamcore-sdk/<version>/` | StreamCore SDK release notes and SHA256 checksums |
| `streamgate/<version>/` | StreamGate release notes and SHA256 checksums |
| `streamcall/<version>/` | StreamCall release notes, authorization boundary, and SHA256 checksums |

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

StreamCore SDK 演示程序源码和可运行演示包在 [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo) 单独发布。

GitHub 提供 StreamCall 本次 10 个已校验交付包；[Gitee 镜像](https://gitee.com/hbstream/streamcall-downloads/releases/tag/streamcall-server-v1.2.2-endpoint-v1.2.2) 提供其中 9 个官方终端与 SDK 包，大型离线服务端包仅通过 GitHub 提供。官方应用为 Windows EXE/ZIP、Linux x86_64 TGZ 与 Android ARM APK；macOS、iOS、Linux aarch64 和 Windows 服务端不属于本次交付。未导入签名授权时服务端按免费版运行；下载不授予商业 API、SDK 集成或 OEM 权利。旧版本保留。

### 官方入口

- 官网：[https://hbrun.com](https://hbrun.com)
- StreamCore SDK：[https://hbrun.com/products/streamcore-sdk](https://hbrun.com/products/streamcore-sdk)
- StreamGate：[https://hbrun.com/products/streamgate](https://hbrun.com/products/streamgate)
- StreamCall：[https://hbrun.com/products/streamcall](https://hbrun.com/products/streamcall)
- 下载中心：[https://hbrun.com/downloads](https://hbrun.com/downloads)

### 仓库结构

| 目录 | 内容 |
| --- | --- |
| `manifests/` | 最新版本的机器可读索引 |
| `streamcore-sdk/<version>/` | StreamCore SDK 版本说明与 SHA256 校验值 |
| `streamgate/<version>/` | StreamGate 版本说明与 SHA256 校验值 |
| `streamcall/<version>/` | StreamCall 版本说明、授权边界与 SHA256 校验值 |

### 校验下载文件

下载后请使用本元数据仓库对应版本目录中的签名清单和 SHA-256 列表校验文件完整性。

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.7.0-windows-x64-standard-installer.exe
```
