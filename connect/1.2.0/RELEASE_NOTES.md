# HBRun Connect 1.2.0 更新说明

本文件说明 `1.2.0` 的版本集合和用户可见边界。实际发布状态、下载文件和校验值以官网对应版本的发行清单为准；不能将本说明反向适用于旧版安装包。

## 机器可读发布集合

```hbrun-connect-release-set-v1
server_linux_x64=1.2.0
connect_admin_linux_x64=1.2.0
expert_windows_x64=1.2.0
field_windows_x64_attended=1.2.0
field_android=1.2.0
web_portal=1.2.0
native_sdk_windows_x64=1.2.0
android_sdk=1.2.0
typescript_sdk=1.2.0
protocol=1.2.0
android_application_id=com.hbr.connect.field
android_version_code=10
```

## 本版产品边界

- 自建 HBRun Connect Server 配合官方 Windows/Android/Web 客户端可长期免费使用，无需申请免费许可证，也不设置商业性的账号、设备、并发会话、使用次数或使用时长额度；实际并发和录像容量仍受服务器、网络、磁盘及运行保护配置约束。
- 官方端的现场视频与语音、现场同意后的录像与下载、有人值守 Windows 远控不因免费模式被裁剪。远控仍需现场人员当次明确同意，可随时停止，不支持无人值守控制、UAC/安全桌面输入或绕过锁屏。
- 客户系统调用 API、Webhook 或集成 SDK 属于另行授权的生产集成；其 60 天申请试用只用于非生产集成评估，并非免费版有效期。OEM/再分发另按合同处理。
- 首次配置应优先引导免费运行；需要集成时由本机管理页生成授权申请资料，导入签名授权后在同一部署上启用集成权益，不要求手工查找部署 ID 或机器标识。
- Android 现场端保留 `com.hbr.connect.field`、`hbrun-connect` 深链及正式品牌；手机桌面使用短标签 `Connect`，应用信息和深链选择器使用完整 `HBRun Connect 现场端`。升级必须沿用原 Connect 发布证书并递增为 `versionCode 10`。

## 部署与信任

- Server 提供 Linux 与 Windows 安装/卸载及本机管理入口；升级前须验证发行身份并备份，失败可回退，默认卸载保留客户数据。首次安装需从可信下载页核对文件大小和 SHA-256；TEST-ONLY 公钥包不能用作正式升级来源。
- 私有部署可生成部署私有 CA，或导入客户/公开 CA；客户端必须信任实际部署证书。公开下载须经 HBRun 官方 HTTPS 来源并对照发行校验清单。
- Windows 仍按产品决定不使用 Authenticode，可能出现“未知发布者”；整包 CMS 不使用。Android APK 必须由 HBRun Connect 独立发布证书签署，Server 发行证明必须由正式授权链签发并由候选工具验签。

发行清单须对应同源构建、正式签名与发行证明，以及该版本的安装和真实协助验收记录。LAN、Debug、TEST-ONLY 或本地官网草稿不等于公开发行版本。
