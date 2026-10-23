<div align="center">
<img src="logo.png" width="180" alt="ResignedPatch logo">

# ResignedPatch

[![Latest Release](https://img.shields.io/github/v/release/real-erm/resignedpatch?label=Release&logo=github)](https://github.com/real-erm/resignedpatch/releases/latest)
[![License](https://img.shields.io/badge/License-GPLv3-blue.svg)](/LICENSE)

</div>

**言語：** [English](./README.md) / [中文](./README_CN.md) / [日本語](./README_JA.md)

**ResignedPatch** (`ermpatch`) は、[FolkPatch](https://github.com/LyraVoid/FolkPatch) および [KernelPatch](https://github.com/LyraVoid/KernelPatch) をベースにしたカスタム Root 管理アプリケーションです。

ResignedPatch の主な目的は、独自の署名識別子（`ermpatch`）とカスタム署名サポートを提供し、開発者やパワーユーザーが上流のハードコードされた署名チェックとの競合なしに、自前のキーでマネージャーを自己署名・デプロイできるようにすることです。

<table>
  <tr>
    <td><img alt="ResignedPatch ホーム画面" src="docs/1.png"></td>
    <td><img alt="ResignedPatch モジュール画面" src="docs/2.png"></td>
    <td><img alt="ResignedPatch 設定画面" src="docs/3.png"></td>
  </tr>
  <tr>
    <td><img alt="ResignedPatch 機能画面" src="docs/4.png"></td>
    <td><img alt="ResignedPatch プラグイン画面" src="docs/5.png"></td>
    <td><img alt="ResignedPatch カスタマイズ画面" src="docs/6.png"></td>
  </tr>
</table>

---

## ResignedPatch の特徴

- **カスタム署名対応 (`ermpatch`)**：公式のハードコードされた署名検証から分離され、自己署名配布を容易にします。
- **独立したビルドパイプライン**：自己署名キーを前提とした設計。
- **完全な FolkPatch エコシステムを継承**：KernelPatch Root、APM システムモジュール、KPM カーネルモジュール、APD Lua プラグイン、各種 UI レイアウトに対応。

## 概要

ResignedPatch は以下を提供します：

- カーネルを再コンパイルせずに利用できる KernelPatch ベースの Root
- カスタム署名識別（`ermpatch`）
- APM システムモジュール（一括インストールおよびバックアップ対応）
- KPM カーネルモジュール（自動読み込み対応）
- 軽量 APD Lua プラグイン
- Shizuku サービスの統合と自動起動
- ネットワーク分離、パス隠蔽、カーネル偽装、マウント隠蔽、アンマウントポリシー
- 各種テーマ、壁紙、カスタムフォント、複数のホームレイアウト
- 多言語対応（英語、中国語、日本語など）

## 動作要件

- ARM64 Android デバイス
- Android カーネルバージョン 3.18 〜 6.15
- サポートされている KernelPatch の導入

## クレジット

- [FolkPatch](https://github.com/LyraVoid/FolkPatch) - マネージャーベース実装・UI
- [KernelPatch](https://github.com/LyraVoid/KernelPatch) - コア Root 実装
- [APatch](https://github.com/bmax121/APatch) - 上流プロジェクト
- [Magisk](https://github.com/topjohnwu/Magisk) - magiskpolicy
- [KernelSU](https://github.com/tiann/KernelSU) - UI およびモジュール構造参照
- [Shizuku](https://github.com/RikkaApps/Shizuku) - 内蔵 Shizuku サービス

## ライセンス

ResignedPatch は [GNU General Public License v3](https://www.gnu.org/licenses/gpl-3.0.html) の下で公開されています。
