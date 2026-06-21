# GitHub Pages Problems

GitHub Pagesで過去に起きた問題や、今後確認すべき原因候補を記録する。

## 表示されない問題

- Live Serverでは表示されるがGitHub Pagesでは表示されない
- CSSのheight指定不足により、地図コンテナの高さが0になる
- ローカルでは動く相対パスが、GitHub Pagesのサブパスでは崩れる
- Mapbox、Leaflet、その他の地図ライブラリの読み込みエラー
- APIキーが必要なサービスで、キーが未設定または制限に引っかかっている
- GitHub Pagesの公開ブランチや公開ディレクトリ設定が違う
- ファイル名の大文字・小文字がローカルとGitHub上で一致していない
- ブラウザconsoleにエラーが出ている

## 原因確認の観点

- `index.html` からCSSとJavaScriptが正しく読めているか
- 地図を表示する要素に高さがあるか
- GitHub PagesのURLに合わせた相対パスになっているか
- 外部CDNが読み込めているか
- 公開ブランチと公開フォルダが正しいか
