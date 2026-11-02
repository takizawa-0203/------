# オバケサーチ PWA版

## 公開方法
このフォルダーの中身を、HTTPS対応のサーバー（GitHub Pages、Netlify、Vercelなど）へそのままアップロードしてください。
Service Workerは `file://` でHTMLを直接開いた場合は動作しません。ローカル確認では localhost を使用してください。

## ローカル確認
このフォルダーで次を実行します。

    python -m http.server 8000

その後、ブラウザーで `http://localhost:8000` を開きます。
Chrome DevToolsの Application から Manifest と Service Workers を確認できます。

## 更新時の注意
ファイルを更新したときは、`sw.js` の `CACHE_NAME` を `obake-search-v2` のように変更してください。

## 画像パス
既存CSSの背景画像は `../img/start_back.png` を参照しています。使用する場合は `img/start_back.png` を追加してください。
