# Analyze App Implementation

指定したGitHubリポジトリのアプリケーション実装を包括的に分析し、技術文書として整理されたHTMLページを生成します。

## Usage
```
/analyze-app <repository-url>
```

## Instructions

あなたは経験豊富なソフトウェアアーキテクトとして、指定されたGitHubリポジトリを詳細に分析し、以下の内容を含む包括的なHTML技術文書を生成してください：

### 1. 基本情報の収集
- リポジトリ名、説明、主要言語
- README.mdの内容分析
- package.json、requirements.txt、build.gradle等の設定ファイル分析
- ライセンス情報

### 2. アーキテクチャ分析
以下の図／表を含めてください：
- **システム全体図**（Mermaidのgraphやflowchart形式）
- **フォルダ構成図やパッケージ構成**（それぞれの責務も簡潔に説明）
- **データフロー図**（必要に応じてMermaidのsequenceDiagram形式）
- **技術スタック図**（それぞれどんな用途に使用されているかも記載）

### 3. 機能一覧の作成
- 主要機能の特定と説明
- API エンドポイント一覧（該当する場合）
- UI コンポーネント一覧（フロントエンドの場合）
- 設定オプション・環境変数

### 4. 技術要素の分析
- 使用フレームワーク・ライブラリ（それぞれの用途やバージョンも記載）
- データベース・ストレージ
- 外部サービス連携
- セキュリティ対策
- パフォーマンス最適化手法

### 5. コード品質評価
- テスト戦略・カバレッジ
- エラーハンドリング
- ロギング・モニタリング
- ドキュメント整備状況

### 6. HTMLページ生成仕様

以下の構造で完全なHTMLページを生成してください：

```html
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[リポジトリ名] - 実装分析レポート</title>
    <script src="https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.min.js"></script>
    <style>
        /* モダンでプロフェッショナルなCSS */
        body { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; line-height: 1.6; margin: 0; background: #f8f9fa; }
        .container { max-width: 1200px; margin: 0 auto; padding: 20px; }
        .header { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 40px 0; text-align: center; }
        .section { background: white; margin: 20px 0; padding: 30px; border-radius: 8px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); }
        .feature-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        .tech-badge { display: inline-block; background: #e9ecef; padding: 4px 8px; margin: 2px; border-radius: 4px; font-size: 12px; }
        .mermaid { text-align: center; margin: 20px 0; }
        h1, h2, h3 { color: #2c3e50; }
        .toc { background: #f8f9fa; padding: 20px; border-radius: 8px; margin-bottom: 30px; }
        .toc ul { list-style: none; padding-left: 20px; }
        .toc a { color: #667eea; text-decoration: none; }
        .highlight { background: #fff3cd; padding: 10px; border-left: 4px solid #ffc107; margin: 10px 0; }
        .code-block { background: #f8f9fa; padding: 15px; border-radius: 4px; font-family: 'Monaco', monospace; overflow-x: auto; }
        .metric { text-align: center; padding: 20px; }
        .metric-value { font-size: 2em; font-weight: bold; color: #667eea; }
        .metric-label { color: #6c757d; }
    </style>
</head>
<body>
    <!-- 完全な分析レポートHTML -->
</body>
</html>
```

### 7. 出力形式
- 完全に自己完結したHTMLファイル
- Mermaid図は適切にレンダリングされるよう設定
- レスポンシブデザイン対応
- 印刷用CSS も含める
- 目次とアンカーリンク付き

### 8. 分析の深度
- コードの静的解析結果
- 依存関係の分析
- セキュリティ上の考慮点
- スケーラビリティの評価
- 保守性の評価

生成されたHTMLは、技術者が実装を理解し、保守・拡張の判断材料として使用できる品質に仕上げてください。
出力には、生成者 (Claude) 情報を含めないようにしてください。

