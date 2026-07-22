# HBRun Downloads

[English](#english) | [简体中文](#简体中文)

## English

This repository publishes release notes, checksums, and machine-readable indexes for HBRun product downloads. Installers and SDK archives are distributed through GitHub Releases.

### Current Releases

| Product | Version | Release |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.3.3 | [streamcore-sdk-v1.3.3](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.3.3) |
| HBRun StreamGate | 1.5.2 | [streamgate-v1.5.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.5.2) |
| HBRun StreamCall | 1.1.1 | [streamcall-v1.1.1](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcall-v1.1.1) |

StreamCore SDK demo source and runnable demo packages are published separately in [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo).

Release assets are also mirrored on [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases). Gitee natively carries the four StreamCall endpoint packages; its StreamCall release page links the exact GitHub server package because that offline archive exceeds Gitee's per-attachment limit. StreamCall Server starts in Free Edition when no signed license is imported; downloading it does not grant Starter, Integration, or OEM rights.

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
Get-FileHash -Algorithm SHA256 .\StreamGate-1.5.2-windows-x64-standard-installer.exe
```

## 简体中文

本仓库公开 HBRun 产品下载所需的版本说明、SHA256 校验值和机器可读索引。安装包与 SDK 压缩包通过 GitHub Releases 分发。

### 当前版本

| 产品 | 版本 | 发布页 |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.3.3 | [streamcore-sdk-v1.3.3](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.3.3) |
| HBRun StreamGate | 1.5.2 | [streamgate-v1.5.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.5.2) |
| HBRun StreamCall | 1.1.1 | [streamcall-v1.1.1](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcall-v1.1.1) |

StreamCore SDK 演示程序源码和可运行演示包在 [hbstream/streamcore-sdk-demo](https://github.com/hbstream/streamcore-sdk-demo) 单独发布。

Release 附件同时镜像到 [Gitee](https://gitee.com/hbstream/hbrun-downloads/releases)。Gitee 原生提供四个 StreamCall 终端包；离线服务端包超过其单附件限制，因此 Gitee 的 StreamCall 发布页链接同一个 GitHub 精确服务端包。StreamCall Server 在未导入签名授权时按免费版运行；下载文件不会授予 Starter、Integration 或 OEM 权利。

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
Get-FileHash -Algorithm SHA256 .\StreamGate-1.5.2-windows-x64-standard-installer.exe
```
