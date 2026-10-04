# Charybdis 4x6 Wireless (Trackball) – ZMK Config

このリポジトリは、**Charybdis 4×6（トラックボール付き）Wireless 版**の **ZMK Firmware 用キー設定（keymap）を管理・ビルドするためのものです。**

* 左右分離 / 4×6 レイアウト
* トラックボール（マウス操作）対応
* Bluetooth（ZMK / nice!nano 等の nRF52 MCU）
* 日本語Windows環境（JIS認識）へのローカライズ対応

---

## 🧩 ハードウェア構成

* **Keyboard**: Charybdis 4×6
* **Firmware**: nRF52 系 (nice!nano 等)
* **接続方式**: Bluetooth（ZMK / split）
* **ポインティングデバイス**: トラックボール内蔵

---

## 🚀 はじめかた（ビルド手順）

### 1. リポジトリの準備
1. このリポジトリを自身のGitHubアカウントに **Fork** してください。
2. Fork したリポジトリの Actions タブを開き、GitHub Actions を有効にします。

### 2. キーマップの編集
本リポジトリの編集は Keymap Editor を推奨します。

---

## 🇯🇵 日本語Windows（JIS認識）へのローカライズ

US配列のCharybdisを、JIS認識設定のWindowsで「刻印通り」に使うためには、外部プロジェクト等を活用してください。

---

## 🧪 GitHub書き込み権限テスト

2026-10-04: ChatGPTからのGitHub書き込みテスト。

---

## 📦 ファームウェアの書き込み

1. GitHub 上のファイルが更新されると、自動的に GitHub Actions でビルドが開始されます。
2. Actions タブから最新のワークフロー実行（Build）を選択します。
3. 画面下部の Artifacts から、ビルドされたファームウェアをダウンロードします。
4. 解凍して得られる .uf2 ファイルを書き込みます。
