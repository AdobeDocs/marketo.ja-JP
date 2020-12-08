---
unique-page-id: 2359791
description: 照会オファーの目標の指定 — Marketto Docs — 製品ドキュメント
title: 照会オファーの目標の指定
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# 照会オファーの目標の指定 {#specify-goal-for-referral-offer}

参照オファーを [作成する場合](create-a-referral-offer.md)、受渡目標を定義する必要があります。 目標は、ページ訪問数やサインアップ数など、Webページ上の個人アクティビティによって定義できます。 カス [タムJavaScriptイベントを使用することもできます](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)。

また、Marketoで [スマートリストトリガー](specify-goal-for-referral-offer.md) （スマート）を使用して、参照者に対してオポチュニティが作成されるなど、マイルストーンを待つこともできます。

目標の例：

* 10回の来訪
* 5参照登録
* 1個の参照されたオポチュニティが作成されました
* 2参照によるeコマース購入
* 5人の参加者によるウェビナー

1. 「 **マーケティングアクティビティ**」に移動します。

   ![](assets/ma.png)

1. 照会オファーを選択し、「ドラフトを **編集」をクリックします。**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 参照オファーエディターで、 **アプリ設定** / **オファーの詳細に移動します。**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 「 **設定**」で、「 **受渡目標** 」ドロップダウンからイベントタイプを選択します。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>「転送者にクレジットを与える **」フロー・ステップを使用する場合は、履行目標タイプとして「** スマートリストトリガー **** 」を選択する必要があります。

* 参照による訪問：オファーの参加者は、オファーをホストする友人からページへの訪問ごとにクレジットを受け取ります。
* 参照先サインアップ：オファーの参加者は、オファーに登録した各友人のクレジットを受け取ります。
* スマートリストトリガー：オファー参加者は、スマートキャンペーンの [スマートリスト](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md) トリガーの条件を満たす各友人のクレジットを受け取り [](http://docs.marketo.com/display/docs/smart+campaigns)ます。 例えば、参照元見込み客がウェビナーにサインアップしたときに起動するトリガーを使用できます。

* カスタムJavaScriptイベント:オファーの参加者は、ページ上で定義されたJavaScriptイベントをトリガーした各友人のクレジットを受け取ります。 カスタムイベントの [コンバージョンスクリプトを参照してください](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>スマートキャンペーンには、ソーシャルアクティビティを監視するための新しいフィルターおよびトリガーが用意されています。 ソーシャルアクティビティでのトリガーとフィルターの [使用を参照してください](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)。

>[!NOTE]
>
>**関連記事**
>
>次に、参照オファーから送信するサインアップ電子メールと受渡通知電子メール [を](send-referral-offer-fulfillment-email.md) 選択します。

