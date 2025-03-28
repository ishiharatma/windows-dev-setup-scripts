# Windows 開発環境セットアップスクリプト

[![🇯🇵 日本語](https://img.shields.io/badge/%F0%9F%87%AF%F0%9F%87%B5-日本語-white)](./README.ja.md) [![🇺🇸 English](https://img.shields.io/badge/%F0%9F%87%BA%F0%9F%87%B8-English-white)](./README.md)

Windows開発環境のセットアップを自動化するPowerShellスクリプトです。必要な開発ツールを一つのスクリプトで素早くインストールできます。

## 含まれるソフトウェア

このスクリプトは以下のソフトウェアを自動的にダウンロードしてインストールします：

1. **Git** - バージョン管理システム
2. **TortoiseGit** - GitのWindowsシェルインターフェース
3. **Google Chrome** - Webブラウザ
4. **WinMerge** - 差分比較・マージツール
5. **Visual Studio Code** - コードエディタ
6. **サクラエディタ** - テキストエディタ
7. **Winshot** - スクリーンショットツール

## 前提条件

- Windows 10/11
- PowerShell 5.1以上
- 管理者権限

## 使用方法

1. スクリプトを`setup-dev-environment.ps1`として保存します
2. PowerShellを管理者として開きます
3. 以下のコマンドを実行してスクリプト実行を許可します：
   ```powershell
   Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
   ```
4. スクリプトが保存されているディレクトリに移動します
5. スクリプトを実行します：
   ```powershell
   .\setup-dev-environment.ps1
   ```

## インストール詳細

- 標準インストーラー形式のソフトウェア（Git、TortoiseGit、Chrome、WinMerge、VSCode、サクラエディタ）はデフォルトの場所にインストールされます。
- ZIP形式のソフトウェア（Winshot）は`C:\tools\[ソフトウェア名]`に展開されます。

## カスタマイズ

以下のようにスクリプトを変更できます：
- ダウンロードURLを更新してソフトウェアのバージョンを変更
- ソフトウェアの追加や削除
- インストールパラメータのカスタマイズ
- インストールディレクトリの変更

## ライセンス

MIT

## 貢献

貢献を歓迎します！プルリクエストをお気軽に提出してください。
