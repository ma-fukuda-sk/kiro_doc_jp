# Server Directory（サーバーディレクトリ）

KiroのMCPサーバーディレクトリについて説明します。サードパーティ統合を通じて機能を拡張できます。

## ディレクトリの内容

以下を含むMCPサーバーのキュレーションされたテーブルを提供：

- Amazon Devices
- AWS Documentation
- Azure
- Chrome DevTools
- Docker
- Git
- GitHub
- Kubernetes
- MongoDB
- PostgreSQL
- その他

各エントリにはインストールリンクと説明が含まれます。

## ワンクリックインストール

カスタム`kiro://`プロトコルリンクを使用して、IDEで設定を事前入力してサーバーを追加できます。

## 重要な注意事項

**警告**: MCPサーバーはサードパーティツールです。信頼できるソースからのみサーバーをインストールし、ドキュメントとライセンスを確認してください。Kiroはサードパーティのl MCPサーバーについて責任を負いません。

## 開発者ツール

インストールリンクを作成するためのヘルパー関数：

### JavaScript/TypeScript

```javascript
const config = { command: "node", args: ["server.js"] };
const encodedConfig = encodeURIComponent(JSON.stringify(config));
const url = `https://kiro.dev/launch/mcp/add?name=my-server&config=${encodedConfig}`;
```

### Python

URL encoding utilities for programmatic link generation

### Bash

`jq`を使用したコマンドライン例

## URLフォーマット

```
https://kiro.dev/launch/mcp/add?name=<server-name>&config=<url-encoded-config>
```

## 追加リソース

- [公式MCP Registry（GitHub）](https://github.com/modelcontextprotocol)
- npm/PyPIパッケージレジストリ
- コミュニティ提供サーバー
