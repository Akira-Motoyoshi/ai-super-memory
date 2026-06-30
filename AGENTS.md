# Codex Instructions

このリポジトリをAI外部記憶として扱う。

## 作業開始時

1. すべての依頼で、最初に `current_context.md` を読む
2. 依頼に関係するプロジェクトを特定する
3. その項目に記載された `Source files` だけを追加で読む
4. `Last verified` から30日以上経過している情報は、確認されるまで現在の事実として断定しない
5. 対象プロジェクトが見つからない場合は `memory_index.md` から必要なファイルを探す

## 編集時

- 変更前に対象ファイルの最新内容を読む
- 既存情報と重複させず、差分を統合する
- 会話ログ全文や未整理の生データを保存しない
- 個人情報、認証情報、秘密情報を保存しない
- 現在の状態が変わった場合は `current_context.md` の Status、Priority、Last verified、Next action、Source filesを更新する
- 新規ファイルを追加した場合は `memory_index.md` を更新する
- 重要な決定は `decisions/decision-log.md` に記録する

## 作業終了時

- 変更内容を簡潔に要約する
- 更新したファイルを列挙する
- 未確認情報や残課題を明示する
- 適切なcommit message案を出す
