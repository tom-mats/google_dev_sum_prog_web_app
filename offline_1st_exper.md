# Offline first experience

* Service workersの話

https://www.youtube.com/watch?v=QiXLaisCq10

## Service workers

* ページとは別のスクリプトを走らせられる
* 閉じてても走る

```
if (navigator.serviceworker) {
  navigator.serviceWoker.registory("./sw.js")
}
```
update worker on reloadをクリックしとけばリロード時に強制的にアップデートしてくれる

ロードの途中にjsをは知らせることができる

## ユースケース

* Responsible resource loader
* レスポンスをキャッシュしてネットワークリクエストなしに返すことができる

## sw-precache

* Googleから提供しているライブラリ
* リストだけ書いておけば，勝手に保存と表示を行ってくれる

  https://github.com/GoogleChrome/sw-precache

## sw-toolbox

* network firstかcache firstかを選択しやすくする

　https://github.com/GoogleChrome/sw-toolbox

## Indexed DB

## Page Shell

* shellはあらかじめキャッシュに保存しておく

## Contents

* Contentはネットワークから取ってくる
