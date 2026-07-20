# StreamCall 0.1.0 Alpha / StreamCall 0.1.0 Alpha 预发行版

## English

This is the authorization-scoped public download channel for StreamCall 0.1.0 Alpha.

### Included downloads

- `StreamCall-Server-Free-0.1.0-alpha-Ubuntu-22.04-x86_64.tar.gz` (Ubuntu 22.04 x86_64 server) - SHA-256 `bbe41119c8b5684113ba1d39c8fb20906f8828f7f1ec369a55b53469c2d7bda9`
- `StreamCall-Endpoint-0.1.0-alpha-Windows-x86_64.zip` (Windows x86_64 endpoint only) - SHA-256 `e402e6141b03c2a1de1e3bbdc35168bdf9483e3ac903425e6eaef8b1bbafdb80`
- `StreamCall-Endpoint-0.1.0-alpha-Linux-x86_64.tgz` (Ubuntu 22.04 x86_64 endpoint only) - SHA-256 `191996fc7dec590046430a39856162fc8a8985597e78a396c19ee6aade56ce8d`
- `StreamCall-Endpoint-0.1.0-alpha-Android-evaluation.apk` (Android evaluation endpoint) - SHA-256 `09b03fd6da23a626820c516b86577b1f8076963fe093f56c6f79b33600c94d7b`

### Authorization and platform boundary

- `public_self_serve_sale_ready=false`. This pre-release opens a Free Edition and signed-evaluation download channel; it does not create a public self-service commercial sale.
- Free Edition needs no license file and is limited to 1 site, 4 total endpoints including at most 1 dispatcher, 2 linked cameras, and 1 concurrent call. It permits only official first-party StreamCall clients.
- Starter, Integration, and OEM rights are not granted by downloading files. A 30-day non-commercial evaluation requires a separately issued signed license; SDK embedding also requires app/package identity binding.
- Ubuntu 22.04 x86_64 is the only supported server platform. Windows and Linux downloads other than the server package are endpoint-only.
- The Android APK is an evaluation/debug-signed first-party terminal. Android AARs, SDK source, Play Store distribution, and customer-app integration are not included.
- macOS is not published because Developer ID signing, notarization, and the current public macOS gate have not passed. iOS remains deferred.
- Combined internal regression packages, the complete Linux sale archive, Starter buyer packages, customer licenses, and all private keys are excluded.

The Windows executable is not Authenticode-signed and the Android APK is not a production store build. Verify every file with the signed manifest before use.

Release public-key SPKI SHA-256: `b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`

## 简体中文

这是 StreamCall 0.1.0 Alpha 按授权边界制作的公开下载渠道。

- `public_self_serve_sale_ready=false`。本次仅开放 Free Edition 和签名评估授权的预发行下载，不代表已经开放自助商业销售。
- Free Edition 无需授权文件，限制为 1 个站点、总计 4 个终端（其中最多 1 个调度席）、2 路关联摄像头、1 路并发呼叫，并且仅允许官方第一方调度中心和终端。
- 下载文件不会自动授予 Starter、Integration 或 OEM 权利。30 天非商业评估需要另行签发的评估授权；把 SDK 集成到客户应用还必须进行应用/包身份绑定。
- 服务端仅支持 Ubuntu 22.04 x86_64。Windows 和独立 Linux 终端包都不包含服务端能力。
- Android 仅发布评估/调试签名的第一方终端 APK，不公开 AAR、SDK 源码、客户应用集成权或应用商店发行能力。
- macOS 因 Developer ID 签名、公证和公开发行门禁尚未通过而不发布；iOS 继续延期。
- 内部组合回归包、完整 Linux 销售归档、Starter 买方包、客户授权文件和私钥均未公开。

Windows 可执行文件尚未进行 Authenticode 签名，Android APK 也不是正式商店构建。使用前必须通过签名清单核对文件完整性。

发布公钥 SPKI SHA-256：`b35858ffe8d5520210b2ea6aa9627cdf90f91c8d7b20452585062e3f77816573`
