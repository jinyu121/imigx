# 极米投影仪 H2 自用固件和 APP

## 精简固件

### 修改内容

1. 开机自动开启 adb
2. 去除所有第三方 APP，精简系统 APP，屏蔽系统升级
3. 精简桌面、去除 AirPlay 投屏广告
4. 恢复出厂设置后依旧是干净系统

### 刷机方法

1. USB 2.0 U 盘格式化为 FAT32
2. 下载固件`GIMI_XHAD01_XHC05_MAXIM_YN_WMP.bin`，放到 U 盘根目录
3. U 盘插到 USB 2.0 （黑色）口上
4. 长按开机键 10 秒开机，自动刷机

可随时使用上述方法安全刷回原厂系统。

## 自制桌面 APP

### 原厂桌面精简版

- 去除所有推荐内容
- 保留视频搜索功能，如已安装相应 APP 可直接进入观看

<img width="1920" height="1080" alt="原厂桌面" src="https://github.com/user-attachments/assets/244ea621-8392-45e1-b108-5e0912953068" />

### Aerial 桌面

- 完美适配遥控器
- 完美对接原厂系统设置、输入源切换、自定义亮度

### CleanYourTV 桌面

- 完美适配遥控器
- 完美对接原厂系统设置、输入源切换

<img width="1920" height="1080" alt="CleanYourTV桌面" src="https://github.com/user-attachments/assets/28cbc63a-5b48-49f1-972a-5f0ebb2e6993" />

### 安装方法

```bash
adb install launcher.apk
```
