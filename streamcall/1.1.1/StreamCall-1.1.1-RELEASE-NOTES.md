# StreamCall Server 1.1.1 / Endpoint 1.1.1

[English](#english) | [简体中文](#简体中文)

## English

This release publishes StreamCall Server 1.1.1 and StreamCall Endpoint 1.1.1. The server and endpoint applications are versioned independently.

### Packages

- **Server 1.1.1:** offline Linux x86_64 package for private deployment, including the browser command center, service administration, calling, and recording.
- **Endpoint 1.1.1:** official applications for Windows x86_64, Linux x86_64, Android arm64-v8a, and macOS x86_64.

### Highlights

- One-to-one audio and video calling between dispatch and field endpoints
- Browser command center for endpoint presence, call handling, and service status
- Call recording, indexed history, and H.264/AAC recording playback
- Private deployment with offline installation, backup, restore, upgrade, and rollback tools
- First-party desktop and mobile applications for dispatch seats and field users

### Deployment and licensing

- The server requires a Linux x86_64 host with Docker Engine and Docker Compose. The offline installer has been validated on Ubuntu 22.04, Debian 12, and Rocky Linux 9. See the [Linux server installation guide](https://hbrun.com/en/articles/streamcall-linux-server-installation/).
- Built-in free capacity supports 1 site, 4 endpoints including up to 1 dispatcher, 2 linked cameras, and 1 concurrent call with official endpoint applications.
- A 30-day non-commercial evaluation, expanded commercial capacity, third-party integration, OEM, and custom delivery require the corresponding signed authorization.
- Official endpoint packages connect to a deployed StreamCall server. They are not server packages and do not include third-party integration SDK rights.

### Platform notes

- The Windows installer is currently unsigned, so Windows may display a publisher warning.
- The Android APK is signed for direct distribution and is not an app-store build.
- The macOS package is a direct-download preview; it is not Developer ID signed or notarized.
- Verify downloaded files against the [signed release metadata](https://github.com/hbstream/hbrun-downloads/tree/main/streamcall/1.1.1).

## 简体中文

本次分别发布 StreamCall 服务端 1.1.1 和 StreamCall 现场终端 1.1.1。服务端与终端独立维护版本号。

### 发布包

- **服务端 1.1.1：** 面向 Linux x86_64 私有化部署的离线包，包含浏览器调度中心、服务管理、呼叫和录制能力。
- **现场终端 1.1.1：** 提供 Windows x86_64、Linux x86_64、Android arm64-v8a 和 macOS x86_64 官方应用。

### 主要能力

- 调度席与现场终端之间的一对一音视频呼叫
- 面向终端在线状态、呼叫处置和服务状态的浏览器调度中心
- 通话录制、索引记录和 H.264/AAC 录像回放
- 支持离线安装、备份、恢复、升级和回滚的私有化部署
- 面向调度席和现场人员的桌面端与移动端官方应用

### 部署与授权

- 服务端需要 Linux x86_64、Docker Engine 和 Docker Compose，离线安装已在 Ubuntu 22.04、Debian 12 和 Rocky Linux 9 上完成验证。部署步骤见 [Linux 服务端安装指南](https://hbrun.cn/articles/streamcall-linux-server-installation)。
- 内置免费容量支持 1 个站点、4 个终端（其中最多 1 个调度席）、2 路关联摄像头和 1 路并发呼叫，仅限官方终端使用。
- 30 天非商用评估、扩展商用容量、第三方集成、OEM 和定制交付需要申请对应的签名授权。
- 官方终端用于连接已部署的 StreamCall 服务端，不能作为服务端使用，也不包含第三方集成 SDK 权利。

### 平台说明

- Windows 安装包当前未进行代码签名，安装时可能显示发布者提示。
- Android APK 已完成直接分发签名，不是应用商店构建。
- macOS 包为直接下载预览版，尚未使用 Developer ID 签名或完成公证。
- 请使用[签名发布元数据](https://github.com/hbstream/hbrun-downloads/tree/main/streamcall/1.1.1)核对下载文件。
