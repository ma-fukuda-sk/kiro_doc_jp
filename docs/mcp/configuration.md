# Configuration（設定）

MCPの設定に関するガイドです。

## 設定ファイル構造

MCPファイルはJSON形式を使用し、ローカルおよびリモートサーバー設定を含む`mcpServers`セクションがあります。

## サーバータイプ

### ローカルサーバー

`command`と`args`プロパティが必要です。

```json
{
  "mcpServers": {
    "my-local-server": {
      "command": "node",
      "args": ["path/to/server.js"]
    }
  }
}
```

### リモートサーバー

`url`プロパティが必要です（本番環境ではHTTPS、localhostではHTTP）。

```json
{
  "mcpServers": {
    "my-remote-server": {
      "url": "https://example.com/mcp"
    }
  }
}
```

## 共通プロパティ

両方のタイプで使用可能：

- `env`: 環境変数
- `disabled`: 無効化フラグ（boolean）
- `autoApprove`: ツール名の配列
- `disabledTools`: 無効化するツールの配列

## 設定場所

### ワークスペースレベル

- パス: `.kiro/settings/mcp.json`
- プロジェクト固有の設定

### ユーザーレベル

- パス: `~/.kiro/settings/mcp.json`
- グローバル設定、すべてのワークスペースに適用

## セットアップ方法

1. **コマンドパレット**: `Cmd+Shift+P`（Mac）/ `Ctrl+Shift+P`（Windows/Linux）
2. **Kiroパネルインターフェース**

## セキュリティベストプラクティス

- 認証情報をハードコーディングする代わりに、`"${API_KEY}"`のような環境変数参照を使用
- 機密性の高い設定をバージョン管理にコミットしない
- 自動承認を有効にする前にツールのパーミッションを確認

## トラブルシューティング

- JSON構文を検証
- コマンドパスがPATHに存在することを確認
- 環境変数名のタイプミスをチェック
- ファイルを保存して変更を適用
