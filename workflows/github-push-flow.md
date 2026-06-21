# GitHub Push Flow

GitHubにcommit/pushする流れ。

## 手順

1. 作業ブランチを作る
   - 例: `bootstrap-super-memory`

2. 既存ファイルを確認する
   - README
   - 関連するmemory card
   - projectファイル

3. ファイルを編集する
   - 重複を避ける
   - 個人情報や秘密情報を含めない
   - MermaidやMarkdownリンクを壊さない

4. 差分を確認する
   - 追加・削除されたファイル
   - 秘密情報が混ざっていないか
   - リンク切れがないか
   - [quality-check.md](quality-check.md) の項目を確認したか

5. commitする
   - 例: `Bootstrap AI super memory structure`

6. pushする
   - 作業ブランチをGitHubにpushする
   - 必要ならpull requestを作る

## 注意点

- `.env`、秘密鍵、トークン、APIキーはcommitしない
- `raw_logs/` はGit管理しない
- 公開リポジトリでも読める内容か確認してからpushする
