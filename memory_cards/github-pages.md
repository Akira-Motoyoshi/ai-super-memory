# GitHub Pages

## 目的

Codexで作成したサイトをGitHub Pagesに公開し、表示不具合を再発防止できるようにする。

## 重要な前提

- Live Serverでは表示されても、GitHub Pagesでは表示されないことがある
- ローカル表示と公開URLでは、パス、読み込み順、公開設定が変わる
- 地図表示では、CSSの高さ指定や外部ライブラリの読み込みが特に重要

## よく使う情報

- 確認項目
  - CSSの `height` 指定
  - 相対パス
  - APIキーの扱い
  - ブラウザのconsole error
  - GitHub Pagesの公開ブランチと公開ディレクトリ設定
  - 地図ライブラリやタイルの読み込みエラー

## 次回AIに読ませるべき内容

- 表示不具合の調査では [projects/github-pages/problems.md](../projects/github-pages/problems.md) を読む
- 次の確認手順は [projects/github-pages/next-actions.md](../projects/github-pages/next-actions.md) を読む
- Codex作業ルールは [codex.md](codex.md) を読む

## 更新ルール

- 解決した問題は、原因と確認方法をセットで追記する
- APIキーやトークンは書かない
- 公開URLやリポジトリ設定は、必要な範囲だけ記録する
