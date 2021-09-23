---
unique-page-id: 4720758
description: リリースノート - 2015年1月 - Marketo ドキュメント - 製品ドキュメント
title: リリースノート - 2015年1月
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 24%

---

# リリースノート：2015年1月 {#release-notes-january}

2015年1月リリースには、次の機能が含まれています。お客様のご契約により、制限やオプションの契約が必要なものがあります。詳細は担当の営業にお問い合わせください。リリース後は、各機能に関する詳細な記事へのリンクを必ずご確認ください。

## マーケティングの自動化の更新 {#marketing-automation-updates}

**モバイル対応のランディングページ**

ランディングページエディター内から、ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md)のモバイルビューを[作成できるようになりました。 デバイスに関係なく効果的にメッセージを配信し、コンテンツを調整して外出先での消費を容易にすることで、エンゲージメントを高めます。 この機能は、リリース後の週を通じて徐々に展開されます。

[ — ランディングページのチュートリアルビデオ —](https://youtu.be/aPQHlG2X6c0)

**新しいRest API呼び出し**

リードおよびアクティビティ ReST API の 3 つの新しい呼び出し：

* リードの削除
* プログラムIDによるリードの取得
* 削除されたリードの取得

また、「リードを同期」には、より高速なAPI呼び出しでリードの変更を非同期で書き込む新しいオプションも用意されています。 詳細は、リリース後に [developers.marketo.com](https://developers.marketo.com) で確認できます

**メールスクリプトのカスタムオブジェクトサポート**

Eメールスクリプト内から、 Accountオブジェクトに関連付けられたカスタムオブジェクトにアクセスできるようになりました。

## リアルタイム パーソナライズ {#real-time-personalization}

**パーソナライズドリマーケティング(GoogleおよびFacebook)**

リマーケティングは、Webサイトを訪問した人に広告を表示します。 リアルタイムパーソナライゼーションのデータを使用して、[Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)と[Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)のリマーケティングキャンペーンをパーソナライズできるようになりました。 様々な業界のオーディエンスにリマーケティングし、アカウントリスト、会社の規模、既知のリードからのデータを指定します。

[名前付きアカウントリストモジュール](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

名前付きアカウントモジュールの機能強化により、ユーザーの一致率と検証機能が向上します。 次の追加が含まれます。

* リードのEメールアドレスを使用した、「名前付きアカウント」リストからの組織の照合（RTPのみの顧客の場合も含む）
* 1アカウントあたり最大100,000件のレコードをサポート
* 表示およびダウンロードするCSVファイルテンプレート

![](assets/image2015-1-14-11-3a12-3a16.png)

**RTPタグオプションの更新**

「アカウント設定」の「RTPタグ」オプションが更新され、次が含まれるようになりました。

1. CDNと非同期（推奨タグ）
1. CDNと同期（高速）
1. CDNを使用しない非同期タグ
1. CDNを使用しない同期タグ

パフォーマンスを最高にするには、Webページのヘッダーの上部で`<head>`の後にタグを配置することをお勧めします。 すべてのタグで、[RTP API](https://developers.marketo.com/documentation/websites/rtp-js-api/)を使用できます。 RTPタグのデプロイ方法について詳しくは、[ここ](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)を参照してください。

![](assets/image2015-1-15-13-3a30-3a45.png)
