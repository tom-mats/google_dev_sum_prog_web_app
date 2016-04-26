# Security for All

httpsの重要度は増している．Service workers はhttps前提

## httpsでないと有効にならないサービス/API

* ホーム画面への追加自体はhttpsではなくてもできるが，サジェストするのはhttpsが必要
* http2
* brotli
* Geolocation...

## ほとんどのサービスはhttpsでないと動かないようになる

### httpsを立てるのは難しい

* localhostはhttpsを使わなくても動く(ローカルだから)
+ httpsをサポートしているクラウドサービスにアップロードする
  * セキュリティのリスクも抑えられる
* cloudflare(http <-> https <-> Users) と中継してくれる
* lets encrypt(freeのhttps証明書提供)
  * 有効期限は短い -> 自動アップデート

### 設定ファイルを書くのも大変

* mozilla ssl config generator
  * 設定内容を書き出してくれる
  * 一番新しいくて安全なのを生成してくれる
* ssl Lab
* chrome のdevtools
