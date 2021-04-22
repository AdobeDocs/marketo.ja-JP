---
unique-page-id: 4720758
description: リリースノート — 2015年1月 —Marketoドキュメント — 製品ドキュメント
title: リリースノート — 2015年1月
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# リリースノート：2015年1月{#release-notes-january}

2015年1月リリースには、次の機能が含まれています。 Marketo版で利用可能な機能を確認してください。 リリース後は、各機能の詳細記事へのリンクを必ず戻して参照してください。

## マーケティング自動化の更新{#marketing-automation-updates}

**モバイル対応ランディングページ**

ランディングページエディター内から[ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md)のモバイル表示を構築できるようになりました。 デバイスに関係なく効果的にメッセージを配信し、外出先での消費を容易にするためにコンテンツをカスタマイズして関与を促進します。 この機能は、リリース後の1週間を通じて徐々に展開される予定です。

[-ランディングページチュートリアルビデオ —](https://youtu.be/aPQHlG2X6c0)

**新しいREST API呼び出し**

リード&amp;アクティビティReST APIの3つの新しい呼び出し：

* リードの削除
* プログラムIDによるリードの取得
* 削除されたリードの取得

また、より高速なAPI呼び出しのために、リードの変更を非同期に書き込むための新しい同期リードのオプションも追加されました。 詳細は、[developers.marketo.com](https://developers.marketo.com)のリリース後に提供されます。

**メールスクリプトのカスタムオブジェクトサポート**

電子メールスクリプト内から、Accountオブジェクトに関連付けられたカスタムオブジェクトにアクセスできるようになりました。

## リアルタイムパーソナライズ {#real-time-personalization}

**パーソナライズドリマーケティング(GoogleおよびFacebook)**

リマーケティングは、Webサイトを訪問した人に広告を表示します。 リアルタイムパーソナライゼーションのデータを使用して、[Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)と[Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)のリマーケティングキャンペーンをパーソナライズできるようになりました。 様々な業界のオーディエンスに再マーケティングし、アカウントリスト、会社の規模、または既知のリードからの任意のデータを指定します。

[名前付きアカウントリストモジュール](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

固有のアカウントモジュールが強化され、ユーザーの一致率と検証が向上します。 追加内容：

* リードの電子メールアドレスを使用して、指定アカウントリストから組織を照合する（RTPのみのお客様の場合も同様）
* アカウントあたり最大100,000件のレコードをサポート
* CSVファイルテンプレートを表示およびダウンロードする

![](assets/image2015-1-14-11-3a12-3a16.png)

**RTPタグオプションの更新**

「アカウントの設定」の「RTPタグ」オプションが更新され、次の項目が含まれるようになりました。

1. CDNと非同期（推奨タグ）
1. CDNと同期（高速）
1. CDNを使用しない非同期タグ
1. CDNを使用しない同期タグ

最良のパフォーマンスを得るために、`<head>`の後のWebページのヘッダーの上部にタグを配置することをお勧めします。 すべてのタグで、[RTP API](https://developers.marketo.com/documentation/websites/rtp-js-api/)の使用が許可されています。 RTPタグを導入する方法の詳細は、[](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)を参照してください。

![](assets/image2015-1-15-13-3a30-3a45.png)
