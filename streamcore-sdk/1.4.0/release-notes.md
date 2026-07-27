# StreamCore SDK 1.4.0

[English](#english) | [简体中文](#简体中文)

## English

StreamCore SDK 1.4.0 adds WHIP (WebRTC publishing) to Professional. The formal Windows packages have been verified with H.264 video, Opus audio, optional Bearer Token authentication, configurable handshake timeout, and RTP packet sizing.

### Highlights

- Added WHIP options to the C API through separate, size-versioned functions without changing the StreamCore 1.x `streamcore_publisher_config_t` binary layout.
- Synchronized the WHIP configuration surface across Android, Apple, and .NET wrappers. The current public WHIP support statement is limited to the verified formal Windows packages.
- Added WHIP target selection and Bearer Token input to the Qt and WinForms demos.
- Selecting WHIP locks the demos to H.264 and Opus, matching the protocol contract.
- Invalid WHIP media codecs return `STREAMCORE_RESULT_UNSUPPORTED_MEDIA_CODEC` (`-6`), with the actual and required codecs included in the error text.
- Existing RTMP, RTSP, SRT, playback, capture, recording, GB28181, and ONVIF public APIs remain unchanged.

### Upgrade Notes

1. Replace the SDK package and runtime libraries together. Do not mix 1.4.0 headers or wrappers with older runtime files.
2. Use the complete WHIP endpoint supplied by the server, with H.264 video and Opus audio.
3. Pass only the token value to the WHIP options; do not add the `Bearer ` prefix yourself.
4. Run preflight before publishing and retain both the result code and error text in application logs.
5. Changing WHIP options while a publisher is running stops the current runtime. Run preflight and start again to apply the new settings.

See `docs/README.md` inside each package for verified platform scope, edition differences, and integration instructions.

## 简体中文

StreamCore SDK 1.4.0 为专业版新增 WHIP（WebRTC 推流）能力。Windows 正式包已完成 H.264 视频、Opus 音频、可选 Bearer Token 鉴权、握手超时和 RTP 包大小配置的真实对端验证。

### 主要更新

- C API 通过独立且带结构大小版本的函数提供 WHIP 参数，不改变 StreamCore 1.x `streamcore_publisher_config_t` 的二进制布局。
- Android、Apple 与 .NET wrapper 已同步 WHIP 配置接口；当前公开的 WHIP 支持范围以经过验证的 Windows 正式包为准。
- Qt 与 WinForms Demo 增加 WHIP 目标选择和 Bearer Token 输入。
- Demo 选择 WHIP 后固定使用 H.264 与 Opus，避免产生协议不接受的编码组合。
- WHIP 编码不兼容时返回 `STREAMCORE_RESULT_UNSUPPORTED_MEDIA_CODEC`（`-6`），错误文本包含实际编码和协议要求。
- 原有 RTMP、RTSP、SRT、播放、采集、录像、GB28181 与 ONVIF 公开接口保持不变。

### 升级要点

1. 同时替换 1.4.0 SDK 包和随包运行库，不要混用旧版头文件、wrapper 或运行库。
2. WHIP 地址使用服务端提供的完整 endpoint，视频使用 H.264，音频使用 Opus。
3. 需要鉴权时只传入 token 内容，不要手工添加 `Bearer ` 前缀。
4. 发布前运行 preflight，并在应用日志中保留返回码和错误文本。
5. 运行中修改 WHIP 参数会停止当前 publisher runtime，需要重新执行 preflight 和 start。

各平台验证范围、版本能力与集成方式以 1.4.0 包内的 `docs/README.md` 为准。
