<div align="center">
<img src="logo.png" width="180" alt="ResignedPatch logo">

# ResignedPatch

[![Latest Release](https://img.shields.io/github/v/release/real-erm/resignedpatch?label=Release&logo=github)](https://github.com/real-erm/resignedpatch/releases/latest)
[![License](https://img.shields.io/badge/License-GPLv3-blue.svg)](/LICENSE)

</div>

**语言：** [English](./README.md) / [中文](./README_CN.md) / [日本語](./README_JA.md)

**ResignedPatch** (`ermpatch`) 是基于 [FolkPatch](https://github.com/LyraVoid/FolkPatch) 和 [KernelPatch](https://github.com/LyraVoid/KernelPatch) 构建的定制化 Root 管理工具。

ResignedPatch 的核心目标是提供一个自带定制签名标识（`ermpatch`）的独立 Root 管理器，支持开发者与高级用户使用自有签名进行构建与部署，摆脱上游硬编码签名和证书校验带来的冲突。

<table>
  <tr>
    <td><img alt="ResignedPatch 首页" src="docs/1.png"></td>
    <td><img alt="ResignedPatch 模块界面" src="docs/2.png"></td>
    <td><img alt="ResignedPatch 设置界面" src="docs/3.png"></td>
  </tr>
  <tr>
    <td><img alt="ResignedPatch 功能界面" src="docs/4.png"></td>
    <td><img alt="ResignedPatch 插件界面" src="docs/5.png"></td>
    <td><img alt="ResignedPatch 自定义界面" src="docs/6.png"></td>
  </tr>
</table>

---

## ResignedPatch 特性

- **自定义签名支持 (`ermpatch`)**：内置定制签名标识，解耦官方硬编码签名校验，方便自签名分发。
- **独立构建流程**：适配自签名密钥，确保管理端与内核补丁无缝联动。
- **保留完整 FolkPatch 生态**：完全兼容 KernelPatch Root、APM 系统模块、KPM 内核模块、APD Lua 插件及现代化 UI（FocusUI 等）。

## 功能概览

ResignedPatch 提供：

- 基于 KernelPatch 的 Root 实现，无需重新编译内核
- 定制签名标识（`ermpatch`）
- APM 系统模块，支持批量安装与备份
- KPM 内核模块，支持自动加载
- 轻量级 APD Lua 插件
- Shizuku 服务管理与开机启动
- 网络隔离、路径隐藏、内核伪装、挂载隐藏与卸载策略
- 主题、壁纸、自定义字体与多种首页布局
- 英语、中文、日语及其他社区翻译

## 前置要求

- ARM64 Android 设备
- Android 内核版本 3.18 至 6.15
- 已安装受支持的 KernelPatch

## 开源致谢

- [FolkPatch](https://github.com/LyraVoid/FolkPatch)：基础管理器与界面实现
- [KernelPatch](https://github.com/LyraVoid/KernelPatch)：核心 Root 实现
- [APatch](https://github.com/bmax121/APatch)：上游项目
- [Magisk](https://github.com/topjohnwu/Magisk)：magiskpolicy
- [KernelSU](https://github.com/tiann/KernelSU)：应用 UI 与模块系统参考
- [Shizuku](https://github.com/RikkaApps/Shizuku)：内置 Shizuku 服务

## 许可证

ResignedPatch 遵循 [GNU General Public License v3](https://www.gnu.org/licenses/gpl-3.0.html)。
