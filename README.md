# HBRun Downloads

<p>
  <a href="#中文说明">中文</a> |
  <a href="#english">English</a>
</p>

## 中文说明

`hbrun-downloads` 用于发布 HBRun StreamCore SDK、HBRun StreamGate 等标准产品下载资产的公开索引、版本说明和校验信息。实际下载文件通过 GitHub Releases 提供。

### 当前产品

| 产品 | 最新版本 | Release |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.3.2 | [streamcore-sdk-v1.3.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.3.2) |
| HBRun StreamGate | 1.5.1 | [streamgate-v1.5.1](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.5.1) |

### 官方入口

- HBRun 官网：[https://hbrun.com](https://hbrun.com)
- StreamCore SDK 产品页：[https://hbrun.com/products/streamcore-sdk](https://hbrun.com/products/streamcore-sdk)
- StreamGate 产品页：[https://hbrun.com/products/streamgate](https://hbrun.com/products/streamgate)
- 下载页：[https://hbrun.com/downloads](https://hbrun.com/downloads)

### 目录结构

| 目录 | 内容 |
| --- | --- |
| `manifests/` | 可机器读取的产品下载索引 |
| `streamcore-sdk/<version>/` | StreamCore SDK 版本说明和 SHA256 校验 |
| `streamgate/<version>/` | StreamGate 版本说明和 SHA256 校验 |

### 校验下载文件

下载后请使用对应版本目录下的 `checksums.txt` 或 Release 中的 `SHA256SUMS.txt` 校验文件完整性。

PowerShell 示例：

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.5.0-windows-x64-standard.zip
```

## English

`hbrun-downloads` publishes public indexes, release notes, and checksums for standard HBRun StreamCore SDK, HBRun StreamGate, and related product downloads. Downloadable files are distributed through GitHub Releases.

### Current Products

| Product | Latest Version | Release |
| --- | --- | --- |
| HBRun StreamCore SDK | 1.3.2 | [streamcore-sdk-v1.3.2](https://github.com/hbstream/hbrun-downloads/releases/tag/streamcore-sdk-v1.3.2) |
| HBRun StreamGate | 1.5.1 | [streamgate-v1.5.1](https://github.com/hbstream/hbrun-downloads/releases/tag/streamgate-v1.5.1) |

### Official Links

- HBRun website: [https://hbrun.com](https://hbrun.com)
- StreamCore SDK product page: [https://hbrun.com/products/streamcore-sdk](https://hbrun.com/products/streamcore-sdk)
- StreamGate product page: [https://hbrun.com/products/streamgate](https://hbrun.com/products/streamgate)
- Downloads: [https://hbrun.com/downloads](https://hbrun.com/downloads)

### Layout

| Directory | Contents |
| --- | --- |
| `manifests/` | Machine-readable product download indexes |
| `streamcore-sdk/<version>/` | StreamCore SDK release notes and SHA256 checksums |
| `streamgate/<version>/` | StreamGate release notes and SHA256 checksums |

### Verify Downloads

After downloading a package, verify it with the matching `checksums.txt` file or the `SHA256SUMS.txt` file attached to the release.

PowerShell example:

```powershell
Get-FileHash -Algorithm SHA256 .\StreamGate-1.5.0-windows-x64-standard.zip
```
