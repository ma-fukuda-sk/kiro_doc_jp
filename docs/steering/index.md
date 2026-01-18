# Steering

Steeringは、マークダウンファイルを通じてKiroにワークスペースに関する永続的な知識を提供します。

## Steeringとは？

Steeringは、マークダウンファイルを通じてKiroにワークスペースに関する永続的な知識を提供する機能です。

## 主な利点

- **Consistent Code Generation（一貫したコード生成）**: プロジェクトの規約に従ったコード生成
- **Reduced Repetition（繰り返しの削減）**: 同じ指示を何度も繰り返す必要がない
- **Team Alignment（チームの整合）**: チーム全体で一貫した開発プラクティス
- **Scalable Project Knowledge（スケーラブルなプロジェクト知識）**: プロジェクトの成長に伴う知識の拡張

## Steeringファイルのスコープ

3つの配置オプション：

### Workspace Steering（ワークスペースsteering）

- 場所: `.kiro/steering/`
- ワークスペース固有の設定

### Global Steering（グローバルsteering）

- 場所: `~/.kiro/steering/`
- すべてのワークスペースに適用

### Team Steering（チームsteering）

- MDM/グループポリシーを通じて配布される集中管理ファイル

## 基本的なSteeringファイル

3つの自動生成テンプレート：

1. **product.md** - プロダクトの目的と目標
2. **tech.md** - 技術スタックのドキュメント
3. **structure.md** - ファイル構成と規約

## カスタムSteeringファイルの作成

1. スコープの選択
2. ファイル名の設定
3. 内容の記述
4. オプションで改善

## AGENTS.mdサポート

AGENTS.mdファイルはマークダウン形式で、inclusion modesをサポートせず、常にインクルードされます。

## Inclusion Modes（インクルードモード）

3種類：

1. **Always included（常にインクルード）**: デフォルト
2. **Conditional inclusion（条件付きインクルード）**: fileMatchパターン
3. **Manual inclusion（手動インクルード）**: `#steering-file-name`でオンデマンド

## ファイル参照

`#[[file:<path>]]`構文を使用してワークスペースファイルをライブリンク。

## ベストプラクティス

- フォーカス
- 明確な命名
- コンテキストの説明
- 例の提供
- セキュリティ
- メンテナンス

## 一般的な戦略

5つのユースケース例：

- API標準
- テスト
- コードスタイル
- セキュリティ
- デプロイメント
