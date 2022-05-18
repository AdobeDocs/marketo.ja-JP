---
unique-page-id: 10097867
description: ウェブパーソナライズアクティビティのスマートリストを定義する - Marketo ドキュメント - 製品ドキュメント
title: ウェブパーソナライズアクティビティのスマートリストを定義する
exl-id: 9987f922-f50c-47b3-aef6-230326b094fc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '299'
ht-degree: 100%

---

# ウェブパーソナライズアクティビティのスマートリストを定義する {#define-a-smart-list-for-web-personalization-activities}

スマートキャンペーンでスマートリストを定義する際に、フィルターおよびトリガーでウェブパーソナライズアクティビティを使用できます。ここでは、ウェブパーソナライズのコールトゥアクション（キャンペーン）をクリックしたすべてのユーザーを取り込みます。

トリガーを使用して、メールやアラートを送信したり、ウェブパーソナライズのコールトゥアクションにエンゲージした訪問者に基づいて値やスコアを変更したりします。また、ウェブパーソナライズのコールトゥアクションをクリックしたリードをフィルタリングして表示することもできます。

1. スマートキャンペーンで、「**スマートリスト**」タブをクリックします。

   ![](assets/image2016-2-9-10-3a49-3a18.png)

   >[!NOTE]
   >
   >スマートリストはとても便利です。詳しくは、[スマートリストの詳細](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を参照してください。

1. トリガーを検索し、キャンバスにドラッグ&amp;ドロップします。

   ![](assets/image2016-6-8-9-3a24-3a24.png)

   >[!NOTE]
   >
   >トリガーを使用したスマートキャンペーンは、トリガーモードで実行されます。トリガーされたイベントと追加されたフィルターに基づいて、1 人につき一度ずつ実行されます。

1. ドロップダウンをクリックし、演算子を選択します。

   ![](assets/image2016-6-7-11-3a10-3a8.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーを示します。修正されない場合、キャンペーンは無効になり、実行されません。

1. トリガーを定義します。

   ![](assets/image2016-6-7-11-3a12-3a23.png)

1. 必要に応じて、フィルターを追加します。

   ![](assets/image2016-6-7-11-3a14-3a20.png)

   >[!TIP]
   >
   >トリガーとフィルターの両方を含むスマートキャンペーンでは、トリガーが一番上に表示されます。トリガーされると、フィルター条件を満たす人のみがフローを通過します。

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、いずれかのトリガーが有効化されると、フローに進みます。

   一連のリードに対してキャンペーンを同時に実行するには、[スマートキャンペーンのスマートリストを定義する | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [予測コンテンツアクティビティのスマートリストの定義](/help/marketo/product-docs/predictive-content/define-a-smart-list-for-predictive-content-activities.md)

