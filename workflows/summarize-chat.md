# Summarize Chat Workflow

ChatGPTやCodexの会話を保存用に要約するテンプレート。

## 原則

- 会話ログ全文は保存しない
- 保存するのは、次回以降に再利用できる要点だけ
- 個人情報、APIキー、メール本文、URLの機密情報は除外する

## 要約テンプレート

```md
# Chat Summary

Date:
Topic:

## 1. 何を相談したか
-

## 2. 決まったこと
-

## 3. 次にやること
-

## 4. 長期記憶に残すこと
-

## 5. プロジェクト記憶に残すこと
-

## 6. 更新すべきファイル
-

## 7. 保存しない情報
-
```

## 分類の目安

- 価値観や判断基準は `memory_cards/`
- 現在進行中の作業は `current_context.md`
- 特定プロジェクトの内容は `projects/`
- 運用ルールは `workflows/`
- 重要な設計判断は `decisions/decision-log.md`
