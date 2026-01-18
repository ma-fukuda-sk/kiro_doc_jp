# Kiro CLI インストールガイド

複数のプラットフォームでのKiro CLIのインストール方法を説明します。

## インストール方法

### macOS

シンプルなワンライナーインストール：

```bash
curl -fsSL https://cli.kiro.dev/install | bash
```

### Linux AppImage

ポータブルフォーマット：

1. AppImageファイルをダウンロード
2. `chmod +x`で実行可能にする
3. アプリケーションを直接実行

### Linux（Zipフォーマット）

システム検証と手動展開が必要：

- glibc 2.34+用と古いバージョン用musl版の別々のダウンロード

### Ubuntu

`.deb`パッケージインストール：

```bash
wget <package-url>
sudo dpkg -i <package-name>.deb
```

## システム要件

「Kiro for command lineはglibc 2.34以降が必要で、これは2021年以降にリリースされたほとんどの主要Linuxディストリビューションにデフォルトで含まれています。」

古いシステムにはmuslベースのバージョンが利用可能です。

### サポートアーキテクチャ

- 64-bit x86_64
- ARM aarch64

### サポートディストリビューション

- Fedora
- Ubuntu
- Amazon Linux 2023

## エンタープライズ機能

CLI（v1.8.0+）にはプロキシサーバーサポートが含まれ、以下の環境変数設定が可能：

- HTTP/HTTPSプロキシ
- 認証資格情報
- ドメインバイパスルール

## トラブルシューティング

問題を診断するには：

```bash
kiro-cli doctor
```

### よくある問題

- 認証失敗
- オートコンプリートの問題
- SSH統合

### サポート

永続的な問題は以下で報告：

```bash
kiro-cli issue
```
