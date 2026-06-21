# Update Memory Workflow

会話後に記憶を更新する手順。

```txt
1. 会話の要点を抽出
2. 長期記憶・短期記憶・プロジェクト記憶に分類
3. 重複を確認
4. 既存ファイルに統合
5. mindmapを更新
6. current_context.mdを更新
7. commit messageを作成
8. GitHubにpush
```

## 詳細手順

1. 会話の要点を抽出する
   - 決定事項
   - 進行中の課題
   - 次にやること
   - 再利用できる言い回し

2. 分類する
   - 長期記憶: 価値観、判断基準、基本ルール
   - 短期記憶: 近日中に必要な文脈
   - プロジェクト記憶: 特定プロジェクトの目的、課題、進捗

3. 保存しない情報を除外する
   - APIキー、パスワード、トークン
   - 住所、電話番号、詳細な個人情報
   - メール本文や会話ログ全文
   - 公開リスクが高い選考情報

4. 既存ファイルに統合する
   - 先に関連ファイルを読む
   - 同じ内容を重複して書かない
   - 古い情報は必要に応じて更新する

5. mindmapとcurrent_contextを更新する
   - 全体像が変わる場合は `mindmaps/` を更新する
   - 進行中の目標が変わる場合は `current_context.md` を更新する

6. commit messageを作る
   - 例: `Update memory cards for job hunting context`

7. GitHubへ反映する
   - 差分確認
   - commit
   - push
