# Android Debug Bridge (ADB) 操作手册

**Android Debug Bridge**，简称 ADB，是 Android 平台开发中的一个核心组件，它提供了一种通过命令行接口与 Android 设备进行通信的桥梁。此工具支持多种功能，包括安装和调试应用程序、设备状态检查、文件传输以及执行设备上的 shell 命令等。以下是使用 ADB 的关键步骤和常用命令的详细说明。

## 1. 环境配置

### 1.1 安装 ADB
1. 访问 [Android SDK Platform Tools](https://developer.android.com/studio/releases/platform-tools) 页面，下载最新版本的 `platform-tools`。
2. 解压缩下载的 ZIP 文件到你的开发环境路径，通常包含 `adb.exe` 及其他相关工具，这一步操作见[【adb】--- win11 配置 adb环境 超详细 （持续更新中）](https://blog.csdn.net/weixin_44205779/article/details/128215134?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522171785530116800226525318%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=171785530116800226525318&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-2-128215134-null-null.142^v100^pc_search_result_base3&utm_term=win11%E5%AE%89%E8%A3%85adb&spm=1018.2226.3001.4187)

### 1.2 连接设备
1. 在 Android 设备上：
   - 进入 **开发者选项** ，开启 **USB调试**。
   - 根据设备型号，可能需要在 **安全设置** 中允许电脑的调试权限。
2. 使用 USB 数据线将设备连接到电脑。
3. 当设备提示授权请求时，确认允许电脑进行调试。

### 1.3 安装 USB 驱动
确保你的电脑已安装了适用于所连接设备的官方 USB 驱动。在设备管理器中检查设备是否被正确识别。

## 2. ADB 命令行操作

### 2.1 列出连接的设备
```bash
adb devices


### 2.2 安装应用
adb install [-r] <path_to_apk>