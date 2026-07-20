# HBRun Downloads

[English](#english) | [简体中文](#简体中文)

## English

This repository publishes release notes, checksums, and machine-readable indexes for HBRun product downloads. Installers and SDK archives are distributed through GitHub Releases.

### Current Releases

| Product | Version | Release |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.3.3 | [streamcore-sdk-v1.3.3](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.3.3) |
| HBRun StreamGate | 1.5.2 | [streamgate-v1.5.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.5.2) |
| HBRun StreamCall | 0.1.0 Alpha | [streamcall-v0.1.0-alpha](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcall-v0.1.0-alpha) |

StreamCore SDK demo source and runnable demo packages are published separately in [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo).

Release assets are also mirrored on [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases). StreamCall is an alpha Free Edition/signed-evaluation download channel; downloading it does not grant Starter, Integration, or OEM rights.

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

Compare the downloaded file with `SHA256SUMS.txt` attached to the release or the matching `checksums.txt` in this repository.

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.5.2-windows-x64-standard-installer.exe
```

## 简体中文

本仓库公开 HBRun 产品下载所需的版本说明、SHA256 校验值和机器可读索引。安装包与 SDK 压缩包通过 GitHub Releases 分发。

### 当前版本

| 产品 | 版本 | 发布页 |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.3.3 | [streamcore-sdk-v1.3.3](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.3.3) |
| HBRun StreamGate | 1.5.2 | [streamgate-v1.5.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.5.2) |
| HBRun StreamCall | 0.1.0 Alpha | [streamcall-v0.1.0-alpha](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcall-v0.1.0-alpha) |

StreamCore SDK 演示程序源码和可运行演示包在 [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo) 单独发布。

Release 附件同时镜像到 [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases)。StreamCall 当前是 Alpha 版 Free Edition/签名评估授权下载渠道；下载文件不会授予 Starter、Integration 或 OEM 权利。

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

下载后请使用 Release 附带的 `SHA256SUMS.txt` 或本仓库对应版本的 `checksums.txt` 校验文件完整性。

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.5.2-windows-x64-standard-installer.exe
```
