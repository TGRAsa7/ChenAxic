# <img src="assets/logo.jpg" width="40" align="top"/> ChenAxic — Android 线刷 / 刷机工具

[![简体中文](https://img.shields.io/badge/语言-简体中文-brightgreen)](./README.md) [![English](https://img.shields.io/badge/语言-English-blue)](./README_EN.md)

基于 **Jetpack Compose + MIUIX（HyperOS 风格）** 的 Android 刷机工具，支持 **Fastboot / ADB / 9008 (EDL)** 多种模式。

## ⚠️ 不开源声明

> 本项目为**闭源软件**，禁止反编译、衍生开发或任何商业用途。

---

## 📋 项目信息

| 项 | 值 |
|---|---|
| 包名 | `com.ChenXluk.org` |
| UI | Jetpack Compose + **MIUIX**（HyperOS 组件库） |
| 要求 | Android 11+（minSdk 30），**需要 root / su** |

---

## 📸 应用截图

<p>
  <img src="assets/screenshots/home.jpg" width="32%"/>
  <img src="assets/screenshots/tools.jpg" width="32%"/>
  <img src="assets/screenshots/qdl_qfil.jpg" width="32%"/>
</p>
<p>
  <img src="assets/screenshots/qdl_partitions.jpg" width="32%"/>
  <img src="assets/screenshots/qdl_log.jpg" width="32%"/>
  <img src="assets/screenshots/detect_9008.jpg" width="32%"/>
</p>
<p>
  <img src="assets/screenshots/detect_fastboot.jpg" width="32%"/>
</p>

---

## 🛠️ 主要功能

### 刷机
- **小米线刷**（MiFlash 式线刷）
- **Fastboot / FastbootD 刷入**
- **ADB Sideload** 刷入
- **欧真加线刷（Oplus Flash）** — 常规线刷 / 纯 FastbootD 线刷（OPPO / Realme / OnePlus，经 fastboot 通道）
- **刷入 KernelSU**
- **高通 QDL（9008 EDL）**——详见下节

### 高通 QDL 面板（9008 EDL）
- **OnePlus VIP 授权** — melf + Digest.elf + Sign.bin 三文件授权
- **OFP/OPS 解包** — 解包 OPPO / OnePlus / Realme 刷机包
- **QFIL 线刷** — 按 rawprogram / patch XML 刷写
- **分区读写** — 刷入 / 提取 / 擦除分区
- **模拟刷写（Dry-run）** — 空跑模拟，不连接设备、不真实刷写
- **AB 分区** — GPT 识别活跃槽位、切换槽位
- **保护机制** — 可跳过 `persist / ocdt / secdata` 与 LUN5、跳过 userdata
- **机型 / 处理器快捷选择** — 自动识别授权类型并填充引导文件

### 设备工具
- **ADB / Fastboot 命令面板**（含常用快捷指令）
- **设备识别 / 设备信息**（品牌、机型、处理器等）
- **重启至多种模式**
- **安装 APK**
- **7z 解压 / payload.bin 解压**
- **内置终端**
- **常用资源链接**（ROM / Recovery / Root 工具合集）

### 个性化
- 多语言（简体中文 / 繁體中文 / English）
- 主题色自定义、壁纸背景、液态玻璃 / 毛玻璃效果

---

## 💡 说明

- 刷机有风险，操作前请自行确认机型与文件匹配，**因使用本工具造成的任何损失由使用者自行承担**
- 本工具仅供个人设备维护与学习使用，**严禁用于非法用途**

---

## 🌐 相关

- [Jetpack Compose 官方文档](https://developer.android.com/jetpack/compose)
- [MIUIX - HyperOS Compose 组件库](https://github.com/miuix-kotlin-multiplatform/miuix)