# StreamCore SDK 1.6.2 发布说明

StreamCore SDK 1.6.2 是授权合同与跨平台交付一致性修复版。媒体公开 ABI、播放、采集、
推流、WHEP、GB28181 和 ONVIF 数据面不变；本版本不在已经稳定的媒体热路径中加入新的
算法或缓存策略。

## 本版变化

- 当前源码和所有打包入口统一报告 `1.6.2`。由于当前主线已经实现 contract v4 平台
  身份合同，CMake 会拒绝把这份源码覆盖打包成低于 1.6.2 的版本；历史版本应从对应的
  不可变源码标签构建。
- Windows / Linux 正式授权绑定实际加载 SDK 的宿主可执行文件名。客户提交文件名，
  不提交安装路径、程序哈希或代码签名主体；授权值由签发端规范化为
  `exe:<basename>`。
- Android 正式授权同时校验 `applicationId` 与发布签名证书 SHA-256。调试签名不能代替
  最终 AAB / APK 的发布签名。
- iOS / macOS 正式授权同时校验 Bundle ID 与 Apple Developer Team ID；完整
  application identifier 由授权服务派生，客户不需要重复填写第三个值。
- Native、Android、Apple 和 .NET 包装层继续由宿主显式提交授权文本；Native 还可显式
  提交授权文件路径。SDK 不扫描安装目录或系统数据目录，也不替客户应用保存授权。
- Demo 与正式 SDK 使用独立的签名密钥、加密 profile 和 envelope domain。Demo 包可以
  公开下载，但 Demo 授权不能被正式 SDK 接受，正式授权也不会被 Demo runtime 当作
  Demo 授权使用。
- 客户授权接入说明已经收敛到 README、平台 README 和公开 API 注释，不再要求客户在
  多份重复文档之间判断优先级。

## 兼容性

- 公开 C ABI 和既有结构体布局不变；现有 1.6.1 集成代码无需因为本次版本升级修改媒体
  调用顺序。
- contract 2 / 3 的历史正式许可证继续按已有兼容合同读取；新签 contract 4 许可证必须
  包含与运行平台一致的 `metadata.target_platform` 和该平台要求的应用身份字段。
- 不得混用不同版本或不同架构的头文件、包装层、静态库、动态库和包元数据。

## 交付验证

1.6.2 正式资产已经过版本、公开 ABI、授权正反例、Demo / 正式 profile 隔离、平台包结构、
依赖闭包、敏感路径、私钥和归档完整性检查。每个下载包均随附平台清单或校验值，客户可在
集成前核对架构、版本和 SHA-256；真实设备与平台运行结论以对应包的 README 和 manifest
所列范围为准。

---

# StreamCore SDK 1.6.2 Release Notes

StreamCore SDK 1.6.2 aligns the licensing contract and cross-platform delivery.
The public media ABI and the playback, capture, publishing, WHEP, GB28181, and
ONVIF data paths are unchanged. No new algorithm or buffering policy is added to
the established media hot path in this maintenance release.

## Changes

- The source tree and package entry points now report `1.6.2`. Because this
  source implements contract-v4 platform identity, CMake rejects packaging it
  as a version below 1.6.2. Historical releases must be built from their
  immutable source tags.
- Windows and Linux licenses bind to the basename of the executable that loads
  the SDK. Customers do not submit an installation path, executable hash, or
  code-signing subject.
- Android licenses validate both the `applicationId` and the production
  release-signing certificate SHA-256.
- iOS and macOS licenses validate the Bundle ID and Apple Developer Team ID.
  The authorization service derives the complete application identifier.
- Hosts continue to register license text explicitly; Native hosts may instead
  provide an explicit license-file path. The SDK neither searches operating
  system directories nor persists customer licenses.
- Demo and production SDKs use independent signing keys, encryption profiles,
  and envelope domains, so a public Demo license is not accepted by the
  production runtime.
- Customer integration guidance is consolidated into the README files and
  public API documentation instead of a separate competing guide.

## Compatibility

- The public C ABI and existing structure layouts are unchanged.
- Historical contract-2 and contract-3 production licenses retain their
  documented compatibility. New contract-4 licenses require a matching
  `metadata.target_platform` and the platform-specific application identity.
- Do not mix headers, wrappers, libraries, or package metadata from different
  versions or architectures.

## Delivery validation

The 1.6.2 assets have passed version, public-ABI, positive and negative license,
Demo/production profile-isolation, platform-layout, dependency-closure,
host-path, private-key, and archive-integrity checks. Each download includes a
platform manifest or checksum so integrators can verify its architecture,
version, and SHA-256 before use. Device and platform runtime claims are limited
to the scope recorded in the matching package README and manifest.
