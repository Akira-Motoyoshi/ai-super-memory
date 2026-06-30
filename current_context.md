# Current Context

Last updated: 2026-06-30

このファイルは、登録済み情報ではなく「現在動いている文脈」を示す。各項目は定期的に確認し、30日以上確認されていない場合は `Status: needs-review` として扱う。

## Active Goals

- GitHub上にAI外部記憶システムを作る
- ChatGPT/Codexの会話で無駄な前提説明を減らす
- マインドマップと記憶カードでワークフローを効率化する
- Codexでファイル更新・commit・pushできる形にする

## Active Projects

### AI Super Memory

- Status: active
- Priority: high
- Last verified: 2026-06-30
- Purpose: このリポジトリ全体を、AIに読ませる外部記憶として整える
- Current context: 会話ログ全文ではなく、要約・分類・記憶カードとして保存し、更新時は既存ファイルを読んでから統合する
- Next action: Codexの起動時参照ルールを運用し、実際の会話で参照漏れがないか確認する
- Source files: `README.md`, `memory_index.md`, `workflows/update-memory.md`, `prompts/codex-startup.md`

### GitHub Pages

- Status: active
- Priority: medium
- Last verified: 2026-06-30
- Purpose: Codexで作成・修正したWebサイトをGitHub Pagesで公開できるようにする
- Current context: Live Serverでは動くがGitHub Pagesでは表示されない問題を、チェックリスト化して再利用する
- Next action: `projects/github-pages/next-actions.md` の確認手順を対象サイトで実行する
- Source files: `memory_cards/github-pages.md`, `projects/github-pages/summary.md`, `projects/github-pages/problems.md`, `projects/github-pages/next-actions.md`

### Codex活用

- Status: active
- Priority: high
- Last verified: 2026-06-30
- Purpose: リポジトリ編集、Markdown整理、GitHub Pages修正、記憶更新案作成にCodexを使う
- Current context: 作業前に既存ファイルを確認し、重複や破壊的な上書きを避ける
- Next action: ルートの `AGENTS.md` と起動プロンプトによる自動参照を検証する
- Source files: `memory_cards/codex.md`, `prompts/codex-startup.md`, `workflows/codex-task-template.md`, `AGENTS.md`

### 就活

- Status: active
- Priority: medium
- Last verified: 2026-06-30
- Purpose: CARTA HOLDINGSなどの企業研究と面接対策に使う
- Current context: マーケティング、広告、デジタル戦略、グローバル展開への関心を整理し、自然でわかりやすい回答を優先する
- Next action: 応募先または次回面接に合わせて企業研究と回答例を更新する
- Source files: `memory_cards/career.md`, `memory_cards/company-mode.md`, `projects/job-hunting/`

### 古橋研究室・GIS/OSM

- Status: active
- Priority: medium
- Last verified: 2026-06-30
- Purpose: GIS、OSM、Re:Earth、YouthMappers、マッピングパーティーなどの活動文脈を整理する
- Current context: 研究、発表、活動報告で再利用できる形に要約する
- Next action: 最新の研究・マッピング活動を確認し、既存の活動記録へ差分を統合する
- Source files: `memory_cards/gis-osm.md`, `memory_cards/research.md`, `projects/furuhashi-lab/`

## ChatGPT / Codex 使用ルール

- 最初にこのファイルを読み、質問に関係する `Source files` だけを追加で読む
- `Status: active` かつ `Priority: high` の項目を優先する
- `Last verified` から30日以上経過した項目は、現在も有効か確認するまで断定に使わない
- 会社モードはオン。仕事・会社・就活・企業研究に関係する会話では、簡潔さ、実務性、相手に伝わる表現、次の行動を優先する
- 既に記憶にある前提を毎回繰り返さない
- 必要なファイルだけ読む
- 作業後に記憶更新案を出す
- 重要な決定は `decisions/decision-log.md` に残す
