# TypeScript/JavaScript開発ガイド

KiroでのTypeScriptとJavaScript開発に関するガイドです。

## 前提条件

- **Node.js**: プラットフォーム用の最新バージョン
- **TypeScript**: TypeScript開発の場合
- **パッケージマネージャー**: npm
- **Git**: バージョン管理

## 推奨拡張機能

- **ESLint**: コード品質
- **Prettier**: フォーマット
- **Auto Rename Tag**: JSX作業
- **JavaScript Snippets**: モダンな開発パターン

## 開発機能

### コード品質分析

Kiroにコードをレビューしてもらい、潜在的なバグ、パフォーマンス問題、スタイル問題を検出できます。

### リファクタリング支援

コードのリファクタリングを支援し、改善を提案します。

### 型提案

既存のJavaScriptコードに基づいてTypeScript型を提案できます。

## Steeringシステム

`.kiro/steering/`に保存されたカスタムsteeringファイルを使用して、プロジェクト固有のコンテキストを提供します。

### 例

- `naming-conventions.md` - 命名規約
- `file-structure.md` - ファイル構造プラクティス
- `react-patterns.md` - Reactベストプラクティスなどのフレームワーク固有パターン

## 自動化機能

Agent hooksにより以下のタスクを自動化：

- ファイル保存時のテスト生成
- TypeScript型チェック
- 依存関係の更新
- ESLint自動修正
- コンポーネントドキュメント生成

## ドキュメントアクセス

`#docs`参照システムで以下のドキュメントに素早くアクセス：

- TypeScript
- Node.js
- React
- Vue.js
- Express
- その他の主要フレームワーク

## デバッグサポート

- **インラインチャット**: `Cmd/Ctrl + I`
- **コンテキスト追加**: `Cmd/Ctrl + L`
- **クイックフィックス**: エラー解決
