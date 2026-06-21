# AI Super Memory

ChatGPT、Codex、GitHubを組み合わせて使うための「AI外部記憶システム」です。

会話ログをそのまま保存する場所ではありません。会話のあとに、必要な情報だけを要約し、分類し、再利用しやすい記憶カードやプロジェクト文脈として残します。

## 目的

- ChatGPTやCodexに毎回同じ前提を説明しなくてよい状態を作る
- 就活、研究、GitHub Pages、Codex、GIS/OSM、大学課題などの文脈を整理する
- 会話内容をそのまま保存せず、要約・分類・記憶カード化する
- Mermaidのマインドマップで全体像を見える化する
- CodexでMarkdownを更新し、GitHubにcommit/pushしやすい運用にする

## 使い方

1. 作業開始時に [current_context.md](current_context.md) を確認する
2. 必要に応じて [memory_index.md](memory_index.md) から関連ファイルを選ぶ
3. ChatGPTやCodexには、必要な記憶カードだけ読ませる
4. 会話や作業のあとに、[workflows/update-memory.md](workflows/update-memory.md) に沿って記憶更新案を作る
5. 更新内容を既存ファイルに統合し、必要ならmindmapも更新する
6. push前に [workflows/quality-check.md](workflows/quality-check.md) で公開リスクを確認する
7. 変更をcommitし、必要に応じてGitHubへpushする

## ディレクトリ構成

```txt
ai-super-memory/
├── README.md
├── profile.md
├── current_context.md
├── memory_index.md
├── mindmaps/
│   ├── main-memory.md
│   ├── job-hunting.md
│   ├── coding.md
│   └── furuhashi-lab.md
├── memory_cards/
│   ├── career.md
│   ├── research.md
│   ├── github-pages.md
│   ├── codex.md
│   ├── gis-osm.md
│   └── writing-style.md
├── projects/
│   ├── github-pages/
│   ├── job-hunting/
│   └── furuhashi-lab/
├── workflows/
│   ├── update-memory.md
│   ├── summarize-chat.md
│   ├── codex-task-template.md
│   ├── github-push-flow.md
│   └── quality-check.md
├── prompts/
│   ├── chatgpt-startup.md
│   ├── codex-startup.md
│   └── memory-update.md
├── .github/
│   └── pull_request_template.md
├── SECURITY.md
├── decisions/
│   └── decision-log.md
└── archive/
    └── old-memory/
```

## 記憶に残す情報

- 長く使う前提、判断基準、作業ルール
- プロジェクトの目的、課題、次の行動
- 面接対策や文章作成で繰り返し使う表現
- GitHub PagesやCodexで起きた問題と解決手順
- GIS/OSM、研究室活動、大学課題の再利用しやすい要約

## 記憶に残さない情報

- APIキー、パスワード、トークン、秘密鍵
- 住所、電話番号、詳細な個人情報
- Zoomリンク、会議URL、非公開メール本文の生データ
- 会話ログ全文、スクリーンショット全文、未整理の生データ
- 公開されると不利になる企業情報や選考情報の詳細

## ChatGPT / Codexでの基本運用

- 最初に [prompts/chatgpt-startup.md](prompts/chatgpt-startup.md) または [prompts/codex-startup.md](prompts/codex-startup.md) を使う
- `current_context.md` を優先し、必要な記憶カードだけ読む
- 既知の情報を長く繰り返さず、差分だけ確認する
- 作業後は [prompts/memory-update.md](prompts/memory-update.md) の形式で更新案を作る
- 重要な決定は [decisions/decision-log.md](decisions/decision-log.md) に残す

## セキュリティ注意点

このリポジトリは公開される可能性を前提に扱います。

- 個人情報は抽象化して書く
- `.env`、秘密鍵、APIキー、トークンは絶対に保存しない
- 生ログを置く場合は `raw_logs/` に入れ、Git管理しない
- 迷った情報は保存せず、要約だけ残す
- push前に差分を確認する
- 漏えい時の対応は [SECURITY.md](SECURITY.md) を確認する
