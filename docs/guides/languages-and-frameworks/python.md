# Python開発ガイド

Kiroは「Pythonプロジェクト向けの強力なAI支援開発機能を提供し、より効率的にコードを書き、デバッグし、保守するのを支援します。」

## 前提条件

- **Python 3.8+**
- **pip**
- **仮想環境ツール**: venv、virtualenv、またはconda
- **Git**: バージョン管理

## サポートされる拡張機能

Open VSX拡張機能との統合：

- **Python**: 言語サポート
- **PyLint**: リンティング
- **Jupyter**: ノートブック
- **Python Debugger (debugpy)**: デバッグ
- **Rainbow CSV**: データファイル処理

## コア機能

### プロジェクトセットアップ

Kiroは設定ファイルの初期化とPythonベストプラクティスに従ったプロジェクト整理を支援します：

- requirements.txt
- .envファイル
- パッケージ構造

### コード分析

以下についてコードをレビュー：

- 潜在的なバグ
- パフォーマンス問題
- PEP 8準拠
- 型ヒントの提案
- リファクタリング改善

### デバッグサポート

- Pythonトレースバックとエラーメッセージの説明
- 一般的なエラーの修正提案
- デバッグツールの設定支援

## Steering & カスタマイズ

`.kiro/steering/`にカスタムsteeringファイルを作成してKiroの動作をガイド：

### 例

- `python-conventions.md` - 命名規約とコードスタイル標準
- `django-patterns.md` - Django固有の開発ガイドライン
- `data-science-patterns.md` - ノートブック構成とMLワークフロー

## Agent Hooks

以下のタスクの自動化hookをサポート：

- ファイル保存時のテスト生成
- 依存関係の更新
- リンティング
- 仮想環境管理

## ドキュメントアクセス

`#docs`参照システムでPythonドキュメントと人気フレームワークに素早くアクセス：

- PyTorch
- PySide6
- その他
