# Introduction to progressive web apps.

## native & the web

通信料はweb browserの方がアプリの二倍

ブラウザを操作するのは10%のみ

Webのシンプルさは重要(urlのみでアクセスできる)

プロセスを踏まえるたびに20%の人が脱落していく

## Slice

SLICE: The Web
https://paul.kinlan.me/slice-the-web/

engagingなサービスを作る.

ユーザーはすぐアクセスできる

### secure

### Linkable

### Indexable

+ 知識を共有していく

### Conposable

### Ephemeral

## Whi do developers need a natvie apps

* performance
* offline access -> Service workers <-今回話した
* periodic background processing
* notification <- 今回話した
* sensors
* os-specific features

## Progressive web apps

* Reliable
* Fast
* engaging

Consistent experience across browsers

### Service workers

Shellはキャッシュに保存されている内容を利用する

コンテンツは取ってくる

### Web app manifests

Contentsはjsonで記載

'''
<link rel="manifests" href="manifests.json"
'''

## full-screen mode

33urlバーなどを表示しない

## Web push notification

* Browerを閉じていてもpushできるようにする

### いろいろなブラウザで動かせるようにする

Service workers : chrome firefox opera OK. Edge, Safariは将来実装予定

# Use case

## Flipkart

* つかう時間が3倍に

http://www.slideshare.net/robnyman/progressive-web-apps-keynote-google-developer-summit-tokyo-japan/
