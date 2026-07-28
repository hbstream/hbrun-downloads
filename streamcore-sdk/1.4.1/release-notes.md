# StreamCore SDK 1.4.1

[简体中文](#简体中文) | [English](#english)

## 简体中文

StreamCore SDK 1.4.1 完善了授权接入与随包文档，并延续 1.4.0 新增的 WHIP（WebRTC 推流）能力。

### 主要更新

- `.lic` 文件和授权文本统一使用同一份加密授权内容，宿主可按平台选择文件读取或文本注册。
- SDK、AAR、XCFramework 和 NuGet 包不内置客户授权；授权由宿主应用在创建媒体会话前读取并注册。
- Android 授权可校验正式包名与签名证书，Apple 授权可校验 Bundle ID、Team ID 和应用标识。
- Windows 专业版继续支持 WHIP（WebRTC 推流），视频使用 H.264、音频使用 Opus；编码不符合要求时返回 `STREAMCORE_RESULT_UNSUPPORTED_MEDIA_CODEC`（`-6`）及明确错误信息。
- 包内 `docs/README.md`、`docs/LICENSE_INTEGRATION.md` 和 `docs/RELEASE_NOTES.md` 均提供完整中文与英文内容。
- 保持 StreamCore 1.x 公共 C ABI 兼容；原有播放、采集、RTMP、RTSP、SRT、录制、GB28181 和 ONVIF 接口不变。

### 升级说明

1. 同时替换目标平台的 1.4.1 头文件、包装层和运行库，不要与旧版本混用。
2. 按包内 `docs/LICENSE_INTEGRATION.md` 由宿主应用导入另行取得的授权。
3. 使用 WHIP 时选择 H.264 视频和 Opus 音频；需要鉴权时只传入 token 内容。
4. 上线前运行 preflight，并保留返回码、错误信息和 SDK 日志用于排查。

各平台的目录结构、能力边界和接入步骤以包内 `docs/README.md` 为准。

## English

StreamCore SDK 1.4.1 improves license integration and packaged documentation while retaining the WHIP (WebRTC publishing) capability introduced in 1.4.0.

### Highlights

- `.lic` files and copied license text now represent the same encrypted license value, allowing each host to choose file loading or text registration.
- SDK archives, AARs, XCFrameworks, and NuGet packages do not contain customer licenses. The host application reads and registers its separately delivered license before creating media sessions.
- Android authorization can validate the production package name and signing certificate. Apple authorization can validate the Bundle ID, Team ID, and application identifier.
- Windows Professional continues to support WHIP (WebRTC publishing) with H.264 video and Opus audio. Unsupported codecs return `STREAMCORE_RESULT_UNSUPPORTED_MEDIA_CODEC` (`-6`) with a specific error message.
- Packaged `docs/README.md`, `docs/LICENSE_INTEGRATION.md`, and `docs/RELEASE_NOTES.md` files contain complete Chinese and English guidance.
- The public StreamCore 1.x C ABI remains compatible. Existing playback, capture, RTMP, RTSP, SRT, recording, GB28181, and ONVIF APIs are unchanged.

### Upgrade Notes

1. Replace the 1.4.1 headers, wrapper, and runtime libraries together for the target platform. Do not mix files from older versions.
2. Let the host application import its separately delivered license as described in `docs/LICENSE_INTEGRATION.md`.
3. Use H.264 video and Opus audio for WHIP. Pass only the token value when authentication is required.
4. Run preflight before deployment and retain result codes, error text, and SDK logs for diagnostics.

See `docs/README.md` inside each package for package layout, capability boundaries, and platform-specific integration steps.
