# AMP

Accelerated Mobile Pages

* wait time > 3s だと40%の人が断念
+ mobile向けのページをみんなで高速化したい

1. PublisherがAMP向けページにを作成する
1. 問題なければ，AMPキャッシュに登録される
1. プラットフォームはAMPキャッシュにデータがあれば，優先的に表示する．

## AMP=現行の技術を利用して，遅くしないようなページを生成する

* Javascriptのコードを直接書き込むのは禁止
* レイアウトはあらかじめ決めておく(imgタグなど)  
  * インラインCSSのみ

## AMPキャッシュに乗った場合

* CDNがクロールしてコピーを生成->データを取りに行くのが早い
* ampキャッシュはhttp/2で通信するので高速

## 作り方

* Structured dataがないとクローラが検索に引っかからない

# Future

* PWAとの連携
  * service workerをインストールさせることはできる
  * まだ実験段階
* Chrome Custom Tabとの連携
