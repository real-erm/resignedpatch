<div align="center">
<img src="logo.png" width="180" alt="ResignedPatch logo">

# ResignedPatch

[![Latest Release](https://img.shields.io/github/v/release/real-erm/resignedpatch?label=Release&logo=github)](https://github.com/real-erm/resignedpatch/releases/latest)
[![License](https://img.shields.io/badge/License-GPLv3-blue.svg)](/LICENSE)

</div>

**Language:** [English](./README.md) / [中文](./README_CN.md) / [日本語](./README_JA.md)

**ResignedPatch** (`ermpatch`) is a customized Android Root management application based on [FolkPatch](https://github.com/LyraVoid/FolkPatch) and [KernelPatch](https://github.com/LyraVoid/KernelPatch). 

The primary goal of ResignedPatch is to provide a clean, self-contained root manager with a custom signature (`ermpatch`), allowing developers and power users to sign, modify, and deploy the manager using their own private keys without conflicting with upstream signature checks or hardcoded fingerprints.

<table>
  <tr>
    <td><img alt="ResignedPatch home screen" src="docs/1.png"></td>
    <td><img alt="ResignedPatch module interface" src="docs/2.png"></td>
    <td><img alt="ResignedPatch settings interface" src="docs/3.png"></td>
  </tr>
  <tr>
    <td><img alt="ResignedPatch feature interface" src="docs/4.png"></td>
    <td><img alt="ResignedPatch plugin interface" src="docs/5.png"></td>
    <td><img alt="ResignedPatch customization interface" src="docs/6.png"></td>
  </tr>
</table>

---

## What's Different in ResignedPatch

- **Custom Signature (`ermpatch`)**: Pre-configured with a custom signature profile, avoiding upstream key conflicts and allowing seamless self-signed deployment.
- **Independent Build Pipeline**: Built to decouple manager authentication from upstream official certificates.
- **FolkPatch Features Maintained**: Retains full compatibility with KernelPatch Root, APM system modules, KPM kernel modules, APD Lua plugins, and modern customizable layouts (FocusUI, ListUI, GridUI, DashboardUI).

## Overview

ResignedPatch provides:

- KernelPatch-based Root without recompiling the kernel
- Custom signature branding (`ermpatch`)
- APM system modules with batch installation and backup support
- KPM kernel modules, including automatic loading
- Lightweight APD Lua plugins
- Shizuku service management and startup integration
- Runtime controls for network isolation, path hiding, kernel spoofing, mount hiding, and unmount policies
- Importable themes, wallpapers, custom fonts, and multiple home layouts
- English, Chinese, Japanese, and additional community translations

## Requirements

- ARM64 Android device
- Android kernel 3.18 through 6.15
- A supported KernelPatch installation

## Modules and Extensions

### APM

APM provides a Magisk-like system module system with installation, removal, enable and disable controls, batch operations, and full backups.

### KPM

KPM provides kernel module support for `inline-hook` and `syscall-table-hook` use cases, including automatic module loading.

### APD Lua Plugins

APD plugins run Lua scripts in the `apd` lifecycle without modifying system files or injecting a kernel module. They support configuration, quick actions, background daemons, and persistent logs.

## Security

The SuperKey and root authorization carry full system privileges. Always keep custom keys secure.

## Credits

- [FolkPatch](https://github.com/LyraVoid/FolkPatch) - base manager implementation & UI
- [KernelPatch](https://github.com/LyraVoid/KernelPatch) - core Root implementation
- [APatch](https://github.com/bmax121/APatch) - upstream project
- [Magisk](https://github.com/topjohnwu/Magisk) - magiskpolicy
- [KernelSU](https://github.com/tiann/KernelSU) - application UI and module system reference
- [Shizuku](https://github.com/RikkaApps/Shizuku) - built-in Shizuku service

## License

ResignedPatch is licensed under the [GNU General Public License v3](https://www.gnu.org/licenses/gpl-3.0.html).
