---
unique-page-id: 4720758
description: リリースノート — 2015年1月 — Marketto Docs — 製品ドキュメント
title: リリースノート — 2015年1月
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# リリースノート：2015年1月 {#release-notes-january}

2015年1月リリースには、次の機能が含まれています。 Marketing Editionで機能が利用できるかどうかを確認してください。 リリース後は、各機能の詳細記事へのリンクを必ず戻して参照してください。

## マーケティング自動化の更新 {#marketing-automation-updates}

**リック・デコスタの新しい写真！**

RickはSmartBear社のMarketo顧客で、 [信じがたい写真を集めています](https://www.flickr.com/photos/rickdecosta)。 見ろ！

## モバイル対応ランディングページ {#mobile-friendly-landing-pages}

ランディングページエディター内からランディングページのモバイル表示を [構築できるようになりました](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) 。 デバイスに関係なく効果的にメッセージを配信し、外出先での消費を容易にするためにコンテンツをカスタマイズして関与を促進します。 この機能は、リリース後の1週間を通じて徐々に展開される予定です。

`<iframe width="420" height="315" src="//www.youtube-nocookie.com/embed/aPQHlG2X6c0" frameborder="0" allowfullscreen></iframe>`

**新しいReST API呼び出し**

リード&amp;アクティビティReST APIの3つの新しい呼び出し：

* リードの削除
* プログラムIDによるリードの取得
* 削除されたリードの取得

また、より高速なAPI呼び出しのために、リードの変更を非同期に書き込むための新しい同期リードのオプションも追加されました。 詳しくは、リリース後、 [developers.marketo.comで詳しく説明します。](http://developers.marketo.com)

**電子メールスクリプティングカスタムオブジェクトのサポート**

電子メールスクリプト内から、Accountオブジェクトに関連付けられたカスタムオブジェクトにアクセスできるようになりました。

## リアルタイムパーソナライゼーション {#real-time-personalization}

**GoogleおよびFacebook向けのパーソナライズされたリマーケティング**

リマーケティングは、Webサイトを訪問した人に広告を表示します。 リアルタイムパーソナライゼーションのデータを [使用して、](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) Google [および](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) Facebookでリマーケティングキャンペーンをパーソナライズできるようになりました。 様々な業界のオーディエンスに再マーケティングし、アカウントリスト、会社の規模、または既知のリードからの任意のデータを指定します。

[名前付きアカウントリストモジュール](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

固有のアカウントモジュールが強化され、ユーザーの一致率と検証が向上します。 追加内容：

* リードの電子メールアドレスを使用して、指定アカウントリストから組織を照合する（RTPのみのお客様の場合も同様）
* アカウントあたり最大100,000件のレコードをサポート
* CSVファイルテンプレートを表示およびダウンロードする

![](assets/image2015-1-14-11-3a12-3a16.png)

RTPタグオプションの更新

[「アカウントの設定」の「RTPタグ](http://docs.marketo.com/display/docs/rtp+tag+implementation) 」オプションが更新され、次の項目が含まれるようになりました。

1. CDNと非同期（推奨タグ）
1. CDNと同期（高速）
1. CDNを使用しない非同期タグ
1. CDNを使用しない同期タグ

最良のパフォーマンスを得るには、の後にWebページのヘッダーの先頭にタグを配置することをお勧めし `<head>`ます。 すべてのタグで [RTP APIを使用できます](http://developers.marketo.com/documentation/websites/rtp-js-api/)。 RTPタグのデプロイ方法の詳細は、 [ここを参照してください](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)。

![](assets/image2015-1-15-13-3a30-3a45.png)
