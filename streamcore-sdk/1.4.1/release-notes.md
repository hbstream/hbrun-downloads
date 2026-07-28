# StreamCore SDK 1.4.1

[简体中文](#简体中文) | [English](#english)

## 简体中文

StreamCore SDK 1.4.1 增加 Windows 专业版 WHIP（WebRTC 推流）支持，并完善跨平台授权接入。

### 主要更新

- Windows 专业版支持 WHIP（WebRTC 推流），视频使用 H.264，音频使用 Opus。
- 编码不符合 WHIP 要求时，返回 `STREAMCORE_RESULT_UNSUPPORTED_MEDIA_CODEC`（`-6`）和对应错误信息。
- Windows、Linux、Android、iOS、macOS 与 .NET 包装层均可通过授权文本注册 License；Native C / C++ 同时保留 `.lic` 文件路径方式。
- 公开 SDK 包不包含客户授权；试用或商业授权单独签发。
- 包内使用说明、授权接入说明和发布说明均提供中文与英文内容。
- StreamCore 1.x 公开 C ABI 保持兼容，现有播放、采集、RTMP、RTSP、SRT、录制、GB28181 和 ONVIF 接口不变。

### 升级提示

1. 同时替换目标平台的 1.4.1 头文件、包装层和运行库，不要混用旧版本文件。
2. 按包内 `docs/LICENSE_INTEGRATION.md` 注册另行取得的授权。
3. 使用 WHIP 时选择 H.264 视频和 Opus 音频。
4. 发布应用前执行 preflight，并检查返回码和错误信息。

2026-07-28 已刷新发布附件中的对客文档，SDK 二进制功能未发生变化。重新下载时请使用当前 `SHA256SUMS.txt` 校验文件。

## English

StreamCore SDK 1.4.1 adds WHIP (WebRTC publishing) to Windows Professional and improves cross-platform license integration.

### Highlights

- WHIP (WebRTC publishing) is available in Windows Professional with H.264 video and Opus audio.
- Unsupported WHIP codecs return `STREAMCORE_RESULT_UNSUPPORTED_MEDIA_CODEC` (`-6`) with an error message.
- Windows, Linux, Android, iOS, macOS, and .NET wrappers support license-text registration. Native C / C++ also retains `.lic` file-path registration.
- Public SDK packages do not contain customer licenses; trial and commercial licenses are issued separately.
- The package README, license integration guide, and release notes are provided in both Chinese and English.
- The public StreamCore 1.x C ABI remains compatible. Existing playback, capture, RTMP, RTSP, SRT, recording, GB28181, and ONVIF APIs are unchanged.

### Upgrade Notes

1. Replace the 1.4.1 headers, wrapper, and runtime libraries together for the target platform. Do not mix files from older versions.
2. Register the separately issued license as described in `docs/LICENSE_INTEGRATION.md`.
3. Use H.264 video and Opus audio for WHIP publishing.
4. Run preflight before releasing the application and inspect result codes and error text.

The release assets were refreshed on 2026-07-28 with revised customer documentation. SDK binary functionality is unchanged. Use the current `SHA256SUMS.txt` when verifying a new download.
