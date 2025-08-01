---
description: Update the README.md file to include design documentation based on the source code and build settings.
---

### README.md の更新

ソースコードやビルド設定ファイルなどを調査し、README.md に設計ドキュメントとしてまとめてください。
特に下記の設計情報は必ず含めるようにしてください。

- プロジェクトの概要
- 主要な成果物と機能の一覧
- ソースコードのパッケージ構成の説明（依存図を含む）
- 技術スタック
- ビルド手順
- GitHub Actions の workflow で定義されているビルド内容のまとめ
- 品質保証

ドキュメントの先頭には、AI による自動生成であることを明記してください（`Claude`という単語は使わないでください）。
既存のドキュメント内容に間違いがある場合は適切に更新してください。
有用性の低い記述内容が見つかった場合は、確認後に削除してください。
記述フォーマットは GitHub Flavored Markdown spec に従い、表や mermaid による図を適宜使用し、簡潔に分かりやすくまとめてください。

### ブラウザでのプレビュー表示

README.md ファイルの更新が済んだら、実際に HTML ファイルを生成して、Web ブラウザ上でプレビュー表示してください。
mermaid の図も正しく表示されるように、CDN 上の mermaid.js を読み込んでレンダリングしてください。

