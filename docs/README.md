# 伊勢宮シフト GitHub Pages 版

## 使い方

1. Apps Script を Web アプリとしてデプロイします。
2. デプロイ済みURL（`/exec` で終わるURL）を `docs/config.js` の `window.SHIFT_API_URL` に入れます。
3. GitHub にこのフォルダを push します。
4. GitHub リポジトリの Settings > Pages で、公開元を `docs` フォルダにします。

## 保存用PIN

Apps Script のスクリプトプロパティに `GITHUB_API_TOKEN` を設定すると、GitHub版から読み込み・保存するときに共有PINを求めます。

スタッフだけで使う場合も、`GITHUB_API_TOKEN` は設定しておくのがおすすめです。
