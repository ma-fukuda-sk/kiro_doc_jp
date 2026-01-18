# Hooks

Agent hooksは、IDE内で特定のイベントが発生したときに、事前定義されたエージェントプロンプトまたはシェルコマンドを実行する自動トリガーです。

## Agent Hooksとは？

Agent hooksは以下のイベントに応答します：

- ファイルの保存
- ファイルの作成/削除
- エージェントターンの完了

### 利点

- コード品質の維持
- 脆弱性の防止
- 手動オーバーヘッドの削減

## Agent Hooksの仕組み

システムは2ステップのプロセスに従います：

1. **Event Detection（イベント検出）**: IDEアクティビティを監視
2. **Automated Action（自動アクション）**: エージェントプロンプトまたはシェルコマンドを実行

## Agent Hooksの設定

### 方法1: Kiroパネルから

1. Agent Hooksセクションで「+」をクリック
2. 自然言語でワークフローを定義
3. Enter/Submitを押す
4. 設定を構成

### 方法2: コマンドパレットから

1. `Cmd + Shift + P`（Mac）または `Ctrl + Shift + P`（Windows/Linux）を押す
2. 「Kiro: Open Kiro Hook UI」と入力

## 詳細ガイド

- [Hook Types（フックタイプ）](./types.md)
- [Hook Actions（フックアクション）](./actions.md)
- [Management（管理）](./management.md)
- [Best Practices（ベストプラクティス）](./best-practices.md)
- [Examples（例）](./examples.md)
