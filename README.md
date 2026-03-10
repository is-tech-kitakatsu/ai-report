# AI Daily News

社内向け AI 最新情報まとめ。毎日自動生成された `YYYY-MM-DD.md` を GitHub Pages で閲覧できます。

## GitHub Pages の設定手順

1. このリポジトリを GitHub に push する
2. リポジトリの **Settings > Pages** を開く
3. **Source** を `Deploy from a branch` に設定
4. **Branch** を `main` / `(root)` に設定して保存
5. しばらくすると `https://<ユーザー名>.github.io/<リポジトリ名>/` で公開される

## 毎日の運用

新しい `YYYY-MM-DD.md` を push すると、GitHub Actions が自動で `manifest.json` を更新します。
サイトには自動的に新しい日付が追加されます。

## ファイル構成

```
.
├── index.html                   # サイト本体（SPA）
├── manifest.json                # 日付一覧（自動更新）
├── 2026-03-10.md                # 日次レポート
└── .github/workflows/
    └── update-manifest.yml      # manifest.json 自動更新 Action
```
