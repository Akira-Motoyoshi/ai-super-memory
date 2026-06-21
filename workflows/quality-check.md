# Quality Check Workflow

記憶更新やGitHub反映の前に確認するチェックリスト。

## 目的

Markdown、Mermaid、リンク、セキュリティの基本確認を行い、公開しても危険が少ない状態にする。

## チェック項目

- [ ] 会話ログ全文を保存していない
- [ ] 個人情報、APIキー、パスワード、メール本文の生データを含めていない
- [ ] `.env`、秘密鍵、トークン類がGit管理に入っていない
- [ ] Markdownのローカルリンクが切れていない
- [ ] Mermaidコードブロックの開始と終了がそろっている
- [ ] `current_context.md` の更新日と進行中の文脈が古くなっていない
- [ ] `memory_index.md` に新規ファイルが反映されている
- [ ] 必要な決定が `decisions/decision-log.md` に残っている

## Codexに頼むときの確認依頼

```md
変更後に以下を確認してください。

- Markdownリンク切れ
- Mermaidコードブロック
- 秘密情報らしき文字列
- 作成・更新ファイル一覧
- commit message案
```
