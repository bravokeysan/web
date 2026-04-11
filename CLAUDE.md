# CLAUDE.md — bravokeysan/web (GitHub Pages)

## プロジェクト概要

きーさんがブラウザで見たい情報をHTMLファイルにまとめ、GitHub Pages (無料・Public) で公開するリポジトリ。

- **公開URL**: `https://bravokeysan.github.io/web/`
- **リモート**: `https://github.com/bravokeysan/web`
- **ブランチ**: `main`（GitHub Pages のソースブランチ）
- **デプロイ**: `main` へのマージで自動反映（数分かかる場合あり）

## ファイル構成

| ファイル | 用途 |
|---|---|
| `index.html` | トップページ |
| `ai_dream_issues.html` | ai-dream-rag リポジトリの GitHub Issues カード一覧 |

## 作業フロー

変更は必ずフィーチャーブランチ → PR → マージの流れで行う。

```
git checkout -b <branch-name>   # ブランチ作成
# 編集
git add <file>
git commit -m "..."
git push -u origin <branch-name>
gh pr create ...                # PR作成
```

## コーディング規約

- HTMLファイルは単一ファイル完結（CSS・JS をインライン）
- 日本語フォント: `"Hiragino Sans", "Yu Gothic", "Noto Sans JP", sans-serif`
- 日本語明朝: `"Hiragino Mincho ProN", "Yu Mincho", "Noto Serif JP", serif`
- タイトル・見出しは日本語で記述する
- `.DS_Store` はコミットしない

## 注意事項

- `main` への直接プッシュは行わない（必ずPR経由）
- コミット・プッシュ・PR作成は確認なしで実行してよい
- `main` へのマージはきーさんが行う（Claudeはマージしない）
- GitHub Pages のデプロイには数分かかるため、マージ後に少し待ってから確認する
