# OnePlus 13 Device Spoofing Magisk Module  
*(适用于修改机型为 OnePlus 13 的 Magisk 模块)*  

![Magisk](https://img.shields.io/badge/Magisk-25.2+-orange?logo=android)  
![Android](https://img.shields.io/badge/Android-11%2B-brightgreen?logo=android)  
![License](https://img.shields.io/badge/License-MIT-blue)  

📌 **项目描述**  
这是一个 Magisk 模块，用于将您的设备型号伪装成 **OnePlus 13**，适用于需要特定设备认证的应用程序或测试场景。  

---

## ✨ 功能特性  
- 将 `ro.product.model` 修改为 `OnePlus 13`  
- 将 `ro.product.device` 修改为 `OnePlus13`  
- 将 `ro.product.manufacturer` 修改为 `OnePlus`  
- **系统级伪装**：通过 `resetprop` 动态修改属性，无需修改系统分区  
- **轻量化**：仅包含必要的脚本和配置  

---

## 📥 安装指南  
1. 下载模块 ZIP 文件：[Releases 页面](https://github.com/Jordy116/MyFirstProject-/releases)  
2. 打开 Magisk Manager → 点击 **模块** → **从存储安装**  
3. 选择下载的 ZIP 文件  
4. 重启设备  

---

## ✔️ 验证是否生效  
在终端或 ADB 中运行以下命令：  
```bash
adb shell getprop ro.product.model    # 应返回 "OnePlus 13"
adb shell getprop ro.product.device   # 应返回 "OnePlus13"
```

---

## ⚠️ 注意事项  
1. **兼容性**：仅支持 Android 11+ 和 Magisk v25.2+  
2. **风险提示**：部分应用可能检测到设备伪装并封禁账号，请谨慎使用  
3. **测试设备**：  
   - OnePlus 8T (Android 13)  
   - Xiaomi Redmi Note 10 (Android 12)  

---

## 📜 开源协议  
MIT License | 详情见 [LICENSE 文件](https://github.com/Jordy116/MyFirstProject-/blob/main/LICENSE)  

---

### 🛠️ 自定义修改提示  
1. 如果模块还修改了其他属性（如指纹 `fingerprint`），请在 **功能特性** 部分补充  
2. 更新 **测试设备** 列表（如果已在其他机型验证通过）  
3. 如需添加截图或演示视频，可插入到 **安装指南** 下方  
