# Java開発ガイド

KiroのAI支援IDEを使用したJava開発の包括的なガイダンスです。

## 前提条件

- **JDK 17以降推奨**（Amazon Corretto推奨）
- **Maven**または**Gradle**
- **Git**: バージョン管理

## 推奨拡張機能

Open VSXから以下をインストール：

- **Extension Pack for Java**
- **Spring Boot Extension Pack**
- **Gradle/Maven管理ツール**

## 開発機能

### プロジェクトセットアップ

Kiroは以下を支援：

- Maven/Gradle設定の作成
- プロジェクト構造の整理
- Spring Bootアプリケーションの適切なレイヤードアーキテクチャの確立

### コード分析

- バグの識別
- パフォーマンス改善の提案
- Builderパターンなどのデザインパターン実装
- Java Streamsの活用

### デバッグ

- エラーメッセージの説明
- 一般的なJava例外の修正提供：
  - NullPointerException
  - ConcurrentModificationException
  - その他

## Steering & 規約

`.kiro/steering/`にカスタムマークダウンファイルを作成してドキュメント化：

### アーキテクチャパターン

- ヘキサゴナルアーキテクチャ
- CQRS
- ドメイン駆動設計（DDD）

### テスト戦略

特定のカバレッジ要件を含むテスト戦略

### エラーハンドリングとパフォーマンスガイドライン

## 高度な機能

### Agent Hooks

以下を自動化：

- JUnitテスト生成
- コード品質チェック（Checkstyle/SpotBugs）
- JavaDoc更新

### MCPサーバー

Maven統合により以下が可能：

- コマンドの実行
- 依存関係の管理
- AI搭載ビルド診断
