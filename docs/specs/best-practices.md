# Best Practices（ベストプラクティス）

Kiro IDEでのSpecs使用に関するベストプラクティスとよくある質問をカバーします。

## 1. 要件のインポート

既存の要件を統合する2つのアプローチ：

- **MCP統合**: MCPサーバーを持つ要件ツールに直接接続
- **手動インポート**: 要件をリポジトリファイルにコピーし、`#filename Generate a spec from it`コマンドを使用

## 2. Specsの反復

Specsシステムは継続的な改善をサポートします：

- `requirements.md`を直接またはspecセッション経由で更新
- `design.md`の「Refine」オプションを使用してドキュメントとタスクを更新
- `tasks.md`の「Update tasks」を使用して新しい要件にマッピングするタスクを作成

## 3. チームでの共有

Specsはバージョン管理されるよう設計されており、チーム全体で簡単に共有できます。

## 4. クロスチームSpecs

推奨事項：

- 専用のspecsリポジトリを作成
- Gitサブモジュールまたはパッケージ参照を使用
- クロスリポジトリレビューワークフローを開発

## 5. VibeからSpecセッションへの移行

vibe会話から「Generate spec.」と言うことでspec生成に移行できます。

## 6. タスクの一括実行

「Run all tasks」ボタンで未完了の必須タスクを同時に実行できます。

## 7. 完了したタスクの処理

2つのオプション：

- `tasks.md`を手動で更新
- Kiroにスキャンして実装済みの機能を識別するよう依頼

## 8. チャットでのSpecs参照

`#spec`コンテキストプロバイダーを使用して、会話にspecファイルを含めます。

## 9. リポジトリごとに複数のSpecs

推奨：1つのモノリシックなspecではなく、異なる機能に対して個別のspecsを作成

### 推奨構造

```
.kiro/specs/
├── user-authentication/
├── product-catalog/
├── shopping-cart/
├── payment-processing/
└── admin-dashboard/
```

### 利点

- 独立した機能作業
- 集中したドキュメント
- 並行チームコラボレーション
