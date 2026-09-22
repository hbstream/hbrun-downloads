# StreamCall Server 1.2.3 / Endpoint 1.2.3 / SDK 1.2.3

发布日期：2026-09-22

## 下载内容

- Linux x86_64 Server 离线部署包，包含调度中心和 Web 终端。
- 官方终端：Windows x64 安装包与绿色包、Linux x86_64 包、Android ARM APK。
- Server SDK：Web 业务接口、事件和浏览器通话集成包。
- Endpoint SDK：Windows x64、Linux x86_64、Android 和 Web 客户应用集成包。

Server 大包仅通过 GitHub 提供；其余九个包可通过 GitHub 或 Gitee 下载。macOS、iOS、Linux aarch64 和 Windows Server 不属于本版交付范围。

## 本版更新

- 完成 Server、官方终端和 SDK 的 1.2.3 版本交付。
- 改进离线部署、升级回滚、录制与回放、诊断和终端交互流程。
- 完成当前交付包的授权隔离、实际设备通话和受影响功能验证。

本版仅面向上述受支持平台，其他平台不提供正式安装包或 SDK。

## 授权说明更正

Server 包内操作手册第 6 节将“业务集成授权”误写为同时包含 Endpoint SDK 集成权益。正确范围见同页提供的《StreamCall 1.2.3 授权说明更正》。业务 API、完整调度 API 和 Endpoint SDK 集成是分别签发的权益；下载 SDK 包不自动授予客户应用集成或再分发权限。交付 Server 包时应同时提供该更正文件。

官方终端可按 Server 的免费或已签发授权使用。客户将 Endpoint SDK 集成到自有应用，还需取得相应权益并登记应用和安装身份。商业授权与 OEM 交付由人工确认，不通过下载动作自动开通。

Windows 应用没有公开的 Authenticode 签名。Android APK 使用发行签名。安装前请核对随页提供的 SHA-256 清单。

## English Summary

This release contains the Linux x86_64 offline Server, official Windows/Linux/Android endpoints, the Web Server SDK, and Windows/Linux/Android/Web Endpoint SDK packages. The Server archive is hosted on GitHub only; the other nine packages are mirrored on Gitee. macOS, iOS, Linux aarch64, and Windows Server are not delivered in this release.

The Server archive's operations manual incorrectly states that Business Integration includes Endpoint SDK rights. Read the accompanying 1.2.3 authorization correction before requesting a license. Business API, Dispatch API, and customer Endpoint SDK integration are separate entitlements. Downloading a SDK does not grant integration or redistribution rights. Check the published SHA-256 values before installation.
