# StreamGate 1.7.0 / Analysis Node 1.1.0

[English](#english) | [简体中文](#简体中文)

## English

StreamGate 1.7.0 is the current stable camera ingest and distribution gateway
release for Windows x64 and Linux x86_64/aarch64. Analysis Node 1.1.0 is an
optional managed component for low-frequency asynchronous video analysis.

### StreamGate packages

- Standard packages run with the long-term free baseline for up to 5 input
  channels without a license.
- Professional packages also start with the same free Standard baseline.
  Professional features require a signed trial or commercial license.
- Windows provides installer and portable ZIP packages. Linux provides
  script-managed `tar.gz` packages for x86_64 and aarch64.
- The media runtime now uses the shared OpenSSL-enabled HBCore FFmpeg build,
  with packaged public CA trust and an explicit private-CA path.

### Analysis Node packages

- One package supports either a StreamGate-managed local installation or an
  outbound-mTLS remote node installation.
- The `base` profile provides image-status and persistent scene-anomaly
  analysis.
- The `ai` profile additionally carries the governed person/vehicle detection
  model and portable ONNX Runtime.
- Windows supports CPU and DirectML execution with observable CPU fallback.
  Linux packages use the portable CPU runtime.
- Analysis Node requires the single signed `video_analytics` entitlement.
  Downloading or installing a package does not grant that entitlement.

### Release boundaries

- Linux aarch64 packages passed cross-build, package, QEMU execution, systemd,
  and production-model compatibility gates. No physical-device throughput or
  real-time capacity claim is made.
- ONVIF Profile G and vendor-recording behavior remain subject to compatible
  device capabilities and field verification.
- Windows installers are currently unsigned. Download from the official
  release and verify SHA-256 before running them.

Use `SHA256SUMS.txt` to verify every downloaded asset.

## 简体中文

StreamGate 1.7.0 是面向 Windows x64、Linux x86_64 和 Linux aarch64 的当前
稳定版摄像头接入与分发网关。Analysis Node 1.1.0 是可选的受管组件，用于低频、
异步的视频智能分析。

### StreamGate 运行包

- 标准版无需申请授权即可长期使用 5 路以内的免费基础能力。
- 专业版运行包在未导入授权时同样按 5 路免费标准能力运行；专业能力需导入签名的
  专业版试用授权或商业授权。
- Windows 提供安装包和便携 ZIP，Linux 提供 x86_64、aarch64 的脚本化
  `tar.gz` 包。
- 媒体运行时已切换到 HBCore 统一的 OpenSSL FFmpeg，随包提供公共 CA 信任材料，
  并支持显式配置私有 CA。

### Analysis Node 安装包

- 同一个安装包可以选择安装为 StreamGate 本机受管组件，或安装为通过 mTLS
  主动连接控制端的远程节点。
- `base` 配置提供画面状态检查和持续场景异常分析。
- `ai` 配置额外包含受治理的人员/车辆检测模型和便携 ONNX Runtime。
- Windows 支持 CPU 和 DirectML，并可在不可用时明确回退到 CPU；Linux 使用
  便携 CPU 运行时。
- Analysis Node 统一使用一个签名的 `video_analytics` 授权项。下载或安装文件
  本身不会获得该项授权。

### 发布边界

- Linux aarch64 已通过交叉构建、安装包、QEMU 执行、systemd 和生产模型兼容性
  门禁，但不据此承诺实体 ARM 设备的吞吐量或实时容量。
- ONVIF Profile G 和厂商录像能力仍取决于兼容设备能力及现场验证结果。
- Windows 安装包当前未进行代码签名，请从官方发布页下载并在运行前核对
  SHA-256。

请使用 `SHA256SUMS.txt` 校验下载文件。
