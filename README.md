# 极米投影仪 H2 自用固件和 APP

基于 H2 原厂固件，面向使用自己安装的应用及 AirPlay 投屏的场景。精简预装软件，减少推荐内容及投屏广告，保留原厂桌面和必要的系统、硬件功能。

## 精简固件

### 预装软件精简

已删除以下预装软件或组件：

| 类别 | 删除内容 |
| --- | --- |
| 第三方视频 | 银河奇异果、芒果 TV、云视听极光、CIBN 聚体育 |
| 广告及统计 | XgimiAdSdk／极米广告服务、酷云、系统日志 DR |
| 语音及麦克风 | 极米语音、离线语音、纯麦 |
| 商店及推荐服务 | 应用市场、主题商城、消息中心、玩机攻略、极米音乐 |
| 物联网及辅助服务 | 小京鱼、物联网服务、投影管家、RemoteDebug |
| 壁纸及场景 | 壁纸模式、任意门／天光云影 |
| 账户及支付 | 极米服务 AccountManager（`com.xgimi.account`）、极米支付 SDK |
| 播放器 | 本地播放器 GimiPlayer |
| 重复投屏组件 | Miracast、投屏 Demo |

- 保留系统设置、资源管理器、极米助手、极米投屏、搜狗输入法、首次开机向导，以及对焦、镜头盖、蓝牙、音频等所需的系统和硬件组件。
- 保留系统保护名单中的原厂桌面、系统升级、个人中心（`com.xgimi.user`）、流媒体核心（`com.xgimi.stream.media`）。

### 其他修改

1. 开机自动开启 adb （端口号：5555）
2. 清理镜像空闲空间并重新压缩，减少刷机包体积约 20%
3. 保留原有分区容量与布局

当前版本不提供 root 权限。

### 刷机方法

1. USB 2.0 U 盘格式化为 FAT32
2. 下载固件`GIMI_XHAD01_XHC05_MAXIM_YN_WMP.bin`，放到 U 盘根目录
3. U 盘插到 USB 2.0 （黑色）口上
4. 长按投影仪机身开机键 10 秒开机，自动刷机

可随时使用上述方法安全刷回原厂系统。

## 自制桌面 APP

### 原厂桌面精简版

- 去除所有推荐内容、视频搜索功能，只留桌面功能
- 去掉左上角的「芒果 TV」图标

<img width="1920" height="1080" alt="原厂桌面" src="https://github.com/user-attachments/assets/244ea621-8392-45e1-b108-5e0912953068" />

### Aerial 桌面

- 完美适配遥控器
- 完美对接原厂系统设置、输入源切换、自定义亮度

<img width="1920" height="1080" alt="Aerial 桌面" src="https://github.com/user-attachments/assets/5c15428c-74bb-4e17-8031-6a7c3fd4021c" />

### CleanYourTV 桌面

- 完美适配遥控器
- 完美对接原厂系统设置、输入源切换

<img width="1920" height="1080" alt="CleanYourTV 桌面" src="https://github.com/user-attachments/assets/28cbc63a-5b48-49f1-972a-5f0ebb2e6993" />

## 修改版 APP

### 投屏

- 关闭已识别的乐播投屏广告，包括投屏开始时的贴片及相关广告展示
- 保留极米投屏及 AirPlay 所需的联网能力
- 保留屏幕镜像、视频投屏及正常连接流程

### 文件管理

- 显示所有文件
- 去除 APK 文件安装限制，禁止 APK 文件被替换为渠道包

### 系统升级

<img width="1920" height="1080" alt="系统升级" src="https://github.com/user-attachments/assets/6a3f0c7f-7904-4e6f-8e62-43a4634d904e" />

- 屏蔽系统升级应用的真实在线版本检查，界面显示「已经是最新系统」。

### 梯形校正

- 去掉「正在校准中，请稍等」的语音提示

## 验证情况

- 精简基线经过多轮 U 盘刷机，已确认能完成首次启动并正常进入系统
- ADB 开机启用已由设备验证
- 修改后的 APP 已验证可以正常使用

## 更多截图

| 项目 | 截图 |
| --- | --- |
| 设置 | <img width="1920" height="1080" alt="设置" src="https://github.com/user-attachments/assets/02b289e1-4eea-4998-8fa0-a2aa434edaf7" /> |
| 系统信息 | <img width="1920" height="1080" alt="系统信息" src="https://github.com/user-attachments/assets/599ffd94-2a29-4a62-a7e6-fa1ac7b61381" /> |
| HDMI 信号源 | <img width="1920" height="1080" alt="信号源" src="https://github.com/user-attachments/assets/1f459aa4-fae7-42b2-93fd-c85385d6d493" /> |
