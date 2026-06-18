# GitHub Pages 公開手順

## 1. Apps Script 側

1. `伊勢宮シフト新/Code.gs` を Apps Script に反映する。
2. スクリプトプロパティに `GITHUB_API_TOKEN` を追加する。
   - これは GitHub 版で読み込み・保存するときの共有PINです。
3. Web アプリとしてデプロイし、`/exec` で終わるURLをコピーする。

## 2. GitHub Pages 側

1. `docs/config.js` を開く。
2. `window.SHIFT_API_URL = '';` の `''` の中に Apps Script の `/exec` URLを入れる。
3. このフォルダを GitHub にアップロードする。
4. GitHub の Settings > Pages で公開元を `docs` フォルダにする。

## 3. 使い方

GitHub Pages のURLを開くと、最初の読み込み時に共有PINを聞かれます。
正しいPINを入れると、GAS側のスプレッドシート保存データを読み書きできます。
