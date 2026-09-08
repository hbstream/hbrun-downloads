# StreamCall Server 1.2.2 / Endpoint 1.2.2 / SDK 1.2.2

Released: 2026-09-08

## Downloads

- Linux x86_64 Server: complete offline deployment archive, including the Web Command Center and Web/PWA endpoint.
- Official endpoints: Windows x64 installer or ZIP, Linux x86_64 TGZ, and Android ARM APK (arm64-v8a and armeabi-v7a).
- Server SDK: JavaScript/TypeScript Web package.
- Endpoint SDK: Windows x64, Linux x86_64, Android, and Web packages.
- macOS, iOS, Linux aarch64, and Windows Server are not included in this release. Previous release assets remain available for historical reference.

The large Server archive is available on GitHub only. Gitee mirrors the other nine packages without changing their bytes. No split archives or download stubs are used.

## Changes

- Hardened SDK JSON, HTTP, text, network, and cancellation error contracts.
- Fixed event-stream cancellation so closing a stream cancels its reader and suppresses further buffered callbacks.
- Added the documented Server SDK streaming recording-download workflow, including signed access and byte ranges.
- Standardized public parameter names and expanded language-appropriate API documentation.
- Completed browser SDK runtime dependency packaging and preservation of required third-party license notices.
- Repackaged the official applications and all SDK targets as 1.2.2.

Verification covered public API contracts, independent customer integrations, SDK host-binding rejection cases, server license rights, and targeted official application installation and call regressions. Earlier full-system and long-duration acceptance evidence was retained for its original packages; a new long-duration run is not claimed for this maintenance release.

## Authorization and Signing

Public download does not grant commercial integration or redistribution rights. The built-in Free Edition supports one site, four endpoints (up to one dispatcher), two linked cameras, and one concurrent call with official clients. Commercial deployment, Business API, Dispatch API, and customer Endpoint SDK rights follow the issued license. Customer SDK hosts must be registered; copying a SDK into another unregistered host does not grant access. Evaluation is free; commercial delivery and OEM arrangements are handled by contact and contract, not self-service checkout.

The Android APK is release-signed for direct distribution. Its signing-certificate SHA-256 is 9e973d2c9f0ec6478313b4c1739c985ef096209a248dc812f85380bf6f6d06ff. Windows applications do not have public Authenticode signing. Verify the package SHA-256 before installation. The Ed25519-signed download manifest authenticates release metadata; it is not Windows code signing, app-store approval, or Apple notarization.

## Chinese Summary

服务端、官方终端、Server SDK 与 Endpoint SDK 本次均为 1.2.2。服务端仅提供 Linux x86_64 离线包；官方应用提供 Windows 安装包/ZIP、Linux TGZ 与 Android ARM APK。SDK 提供独立客户集成包，下载不自动授予商业集成或再分发权限。macOS、iOS、Linux aarch64 与 Windows 服务端不属于本次交付。旧版文件保留。
