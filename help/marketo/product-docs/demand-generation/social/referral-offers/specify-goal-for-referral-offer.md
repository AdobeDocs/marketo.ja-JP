---
unique-page-id: 2359791
description: 照会オファーの目標の指定 — Marketto Docs — 製品ドキュメント
title: 照会オファーの目標の指定
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# 参照オファーの目標を指定{#specify-goal-for-referral-offer}

[参照オファー](create-a-referral-offer.md)を作成する場合は、受渡目標を定義する必要があります。 目標は、ページ訪問数やサインアップ数など、Webページ上の個人アクティビティによって定義できます。 [カスタムJavaScriptイベント](../../../../product-docs/demand-generation/social/social-functions/conversion-script-for-custom-events.md)を使用することもできます。

別の方法として、マーケティングで[スマートリストトリガー](specify-goal-for-referral-offer.md)を使用して、参照者に対してオポチュニティが作成されるなど、マイルストーンを待つこともできます。

目標の例：

* 10回の来訪
* 5参照登録
* 1個の参照されたオポチュニティが作成されました
* 2参照によるeコマース購入
* 5人の参加者によるウェビナー

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/ma.png)

1. 参照オファーーを選択し、「**ドラフトを編集」をクリックします。**

   ![](assets/image2014-9-19-15-3a6-3a35.png)

1. 参照オファーエディターで、**アプリ設定**/**オファーの詳細に移動します。**

   ![](assets/image2014-9-19-15-3a6-3a44.png)

1. 「**設定**」で、**達成目標**&#x200B;ドロップダウンからイベントタイプを選択します。

   ![](assets/image2014-9-19-15-3a6-3a56.png)

>[!TIP]
>
>「**転送者にクレジットを与える**」フローステップを使用する場合は、「**スマートリストトリガー**」をフルフィルメント目標タイプとして選択する必要があります。

* 参照による訪問：オファーの参加者は、オファーをホストする友人からページへの訪問ごとにクレジットを受け取ります。
* 参照先サインアップ：オファーの参加者は、オファーに登録した各友人のクレジットを受け取ります。
* スマートリストトリガー：オファー参加者は、[スマートキャンペーン](http://docs.marketo.com/display/docs/smart+campaigns)の[スマートリスト](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)トリガーの条件を満たす各友人のクレジットを受け取ります。 例えば、参照元見込み客がウェビナーにサインアップしたときに起動するトリガーを使用できます。

* カスタムJavaScriptイベント:オファーの参加者は、ページ上で定義されたJavaScriptイベントをトリガーした各友人のクレジットを受け取ります。 「[カスタムイベント用のコンバージョンスクリプト](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)」を参照してください。

>[!NOTE]
>
>スマートキャンペーンには、ソーシャルアクティビティを監視するための新しいフィルターおよびトリガーが用意されています。 [ソーシャルアクティビティに対するトリガーとフィルターの使用](../../../../product-docs/demand-generation/social/social-functions/triggers-and-filters-for-social-activities.md)を参照してください。

>[!MORELIKETHIS]
>
>次に、参照オファーから送信するサインアップと購読提供数の電子メール](send-referral-offer-fulfillment-email.md)を[選択します。

