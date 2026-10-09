# HBRun Connect 1.1.0 发布说明

HBRun Connect 1.1.0 是当前正式公开交付的统一版本。它面向客户私有部署的远程可视协助与专家支持场景，包含 Linux/Windows Server、Windows 专家端、Windows 有人值守现场端、Android 现场端、Web Portal 以及三类集成 SDK。各组件使用同一产品版本号；底层 realtime wire、Native C ABI、Webhook schema、SQLite schema 和许可证合同继续按各自兼容版本演进，不因产品次版本升级而无故破坏兼容。

> 发布修订 2：修正协议包、客户文档和发布说明中的预发布状态措辞。客户端、Server、SDK 二进制、
> Android 签名证书和 Server release attestation 均未改变；请始终以当前 `release-index.json` 与
> `SHA256SUMS` 为准。

## 机器可读发布集合

```hbrun-connect-release-set-v1
server_linux_x64=1.1.0
connect_admin_linux_x64=1.1.0
expert_windows_x64=1.1.0
field_windows_x64_attended=1.1.0
field_android=1.1.0
web_portal=1.1.0
native_sdk_windows_x64=1.1.0
android_sdk=1.1.0
typescript_sdk=1.1.0
protocol=1.1.0
android_application_id=com.hbr.connect.field
android_version_code=9
```

## 主要能力

- 专家可从 Windows 原生端或辅助 Web Portal 发起/加入可视协助，现场可使用 Android App 或有人值守 Windows 端接入。
- 双向语音、现场摄像头视频、Android 前后摄像头切换、屏幕分享、远程指针与标注均纳入会话生命周期管理。
- 两方浏览器专家与 Android 现场端可在条件允许时使用端到端直连；录像、屏幕共享或扩展参与者需要服务端媒体能力时迁移到 SFU，直连失败保留 SFU 回退。
- 浏览器可显式选择摄像头和麦克风并在会话中安全切换；Android 提供前后镜头切换、运行态媒体指标以及自动/省带宽/清晰质量策略。
- 媒体编码策略仅在平台确认硬件/高效 H.264 时优先使用，并保留 VP8 或浏览器默认回退；运行态 codec、分辨率、帧率、码率和网络路径以实际统计为准。
- Windows 屏幕共享按静态、文字、滚动和视频内容使用 2/5/15/30 fps 与
  300 kbps/600 kbps/1.5 Mbps/3 Mbps 分档；常规协助默认文字档，静止桌面不重复
  发送相同帧，并显示实际发送分辨率、帧率和区间码率，避免把摄像头策略或配置
  上限机械当作桌面实际流量。
- 现场明确同意后可录像；录像状态、失败原因、下载鉴权、范围请求和完成态导出均由服务端控制。
- 有人值守 Windows 现场端提供显式同意、随时停止、审计可见的远程输入控制，不支持无人值守接管或 UAC/安全桌面绕过。
- Server 支持 Linux 与 Windows 私有部署、内建部署私有 CA、HTTPS/WSS、TURN/TLS、升级回滚、默认保留数据卸载和显式清除数据。
- 对接客户系统时提供 REST/OpenAPI、版本化 WSS、签名 Webhook、TypeScript SDK、Android AAR 和 Windows Native C ABI。

## 安装与信任说明

- Windows 安装包 1.1.0 暂不使用 Authenticode。官网下载页和 `CHECKSUMS.sha256` 用于校验下载字节；Windows 仍可能显示“未知发布者”，企业策略也可能阻止未签名程序。
- Android APK 使用独立的 HBRun Connect Android 发布证书签名。后续升级必须继续使用相同证书；不要用 Debug 或其他产品证书覆盖安装。
- 私有部署可由引导程序生成部署级私有 CA，也可导入客户 CA/公开 CA。使用私有 CA 时，客户端必须通过可信管理通道安装根证书。
- GitHub/Gitee 正式发布页通过 HTTPS 提供下载身份与传输保护；本版本不使用 CMS 包签名。

## 兼容与边界

- Android 最低 API 23、目标 API 34，官网 APK 直发；本版本不声明 Google Play 上架兼容性。
- 桌面客户端为 Windows x64；Linux 桌面客户端不在 1.1.0 范围内。
- Windows 仅支持有人值守远控；文件传输、剪贴板同步、无人值守控制和安全桌面输入不在范围内。
- 产品按一个逻辑 Server 部署与一个命名产品/App 家族授予生产集成许可；官方客户端不另行按设备收费。额外逻辑部署、额外产品家族或 OEM 再分发需要扩展授权范围。
- 1.1.0 已完成同一干净来源构建、平台签名/未签名状态核对、候选验收和双镜像匿名回读；开发工作树或较早 1.0.1 制品不能冒充 1.1.0。

## 发布校验

1. 先核对官网下载页公布的文件大小和 SHA-256。
2. Android 安装前核对包名 `com.hbr.connect.field`、版本 `1.1.0`、versionCode `9` 及发布证书 SHA-256。
3. Windows 安装时确认文件来自 HBRun 官方 HTTPS 下载页，并接受本版暂未签名的明确提示。
4. Server 首次配置完成后执行内置健康检查，再将客户端加入地址交付给用户。
