# Examples（例）

開発者がプロジェクトに適応できる実用的なagent hookの実装例を紹介します。各例にはトリガータイプ、ターゲットパターン、完全な指示が含まれます。

## Security Pre-Commit Scanner（セキュリティプリコミットスキャナー）

**トリガー**: Agent Stop

コミット前に変更されたファイルをスキャンし、APIキー、認証情報、暗号化キー、その他の機密データを検出します。

## Centralized User Prompt Logging（集中ユーザープロンプトログ）

**トリガー**: Prompt Submit
**アクション**: Shell Command

分析と監査のためにユーザープロンプトをGrafana Lokiにログ記録します。

## Internationalization Helper（国際化ヘルパー）

**トリガー**: File Save（英語ロケールファイルを監視）

不足している翻訳を識別し、言語ファイル全体で「NEEDS_TRANSLATION」または「NEEDS_REVIEW」としてマークします。

## Test Coverage Maintainer（テストカバレッジメンテナー）

**トリガー**: File Save

- 新しい関数を識別
- テストカバレッジを確認
- 不足しているテストケースを生成
- カバレッジレポートを更新

## Documentation Generator（ドキュメント生成器）

**トリガー**: Manual

- 関数シグネチャを抽出
- パラメータと戻り値の型をドキュメント化
- ドキュメントの一貫性を確保

## MCP統合の例

hookがModel Context Protocol（MCP）を活用して機能を強化する方法を示します。

### Figmaデザイン検証Hook

HTML/CSSがデザインシステムと一致しているかチェックします。

## 関連ドキュメント

- [Hook Actions](./actions.md)
- [Management](./management.md)
