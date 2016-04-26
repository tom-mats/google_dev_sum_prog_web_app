# Instant loading

* Webアプリをすぐに読み込ませる方法
* 最初の画面が何かしら出る(白画面とかではない)

## Service Workersを使えばいい?

* Service workerに最初にキャッシュをさせる時間がかかる
* ContentsやJSの更新を考慮しなくてはならない

## assetsを小さく保つ

* ファイルとしてリクエストされるもの
  * html
  * css
  * js

### Webアプリの読み込みが早ければ，20%のアドバンテージがある

### スピードを上げれば，収益も上がる

## 目標

### 大きすぎなくする
### 必要なものだけダウンロードさせる

+ browsersに合わせてjavascriptを変えるとか
* 読み込みの優先順位

### 変更されたものだけダウンロードさせる

* キャッシュをきちんと動作させる

## データを圧縮させる(gzip)

* minifyされた方を使う
* Webp
* 端末のサイズに応じてきちんとロードするのと分ける

```
srcset
```

### Round trips time

* Wifiでもrequestごとに1rtで 50msぐらいはかかる
　* 最近のページは100requestぐらいあるので層時間で1s弱かかる
  * Redirectを減らす

```
link
rel = "dns-prefetch" <- iosでも対応
rel = "preconnect"
rel = "preload"
rel = "prefetch"
```
## Be interactive

### javascript

<script defer>とか<script async> を使う

### css

非同期に読み込ませる方法もあるが，ダメなwebポクなってしまう

#### Regioning/Critical

Critical: 必須なものだけ読み込ませる
Regioning : 段階的に表示させる(枠組みだけ表示)

## うまくキャッシュを使う

* ファイルにキャッシュ名をつけてあげれば，名前が変わるので変わったかどうかわかりやすい

## CDNs

* 一番近いところからデータを取ってくれる
* http2をサポートしているとなお良い

## http2で不要になるもの

* concatetnation
* sharding
* cookies
