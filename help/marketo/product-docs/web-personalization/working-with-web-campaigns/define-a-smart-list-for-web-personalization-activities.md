---
unique-page-id: 10097867
description: Marketo Engageで、のスマートリストを定義して、web パーソナライゼーションアクティビティのスマートリストを定義する方法を説明します。 このガイドを使用して、次のステップを完了してください。
title: Web パーソナライゼーションアクティビティのスマートリストの定義​
exl-id: 9987f922-f50c-47b3-aef6-230326b094fc
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/hxhAO-zK6QPXwtm93WY951MT9SHKmvFYtja495CDWtM'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 84%
---
# [!DNL Web Personalization] アクティビティのスマートリストを定義 {#define-a-smart-list-for-web-personalization-activities}

スマートキャンペーンでスマートリストを定義する場合、フィルターおよびトリガーで[!DNL Web Personalization] アクティビティを使用できます。 ここでは、[!DNL Web Personalization] のコールトゥアクション（キャンペーン）をクリックしたすべてのユーザを取り込みます。

トリガーを使用して、メールやアラートを送信したり、[!DNL Web Personalization] のコールトゥアクションにエンゲージした訪問者に基づいて値やスコアを変更したりします。 また、[!DNL Web Personalization] のコールトゥアクションをクリックしたリードをフィルタリングして表示することもできます。

1. スマートキャンペーンで、「**[!UICONTROL スマートリスト]**」タブをクリックします。

   ![](assets/image2016-2-9-10-3a49-3a18.png)

   >[!NOTE]
   >
   >スマートリストはとても便利です。 詳しくは、[スマートリストの詳細](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を参照してください。

1. トリガーを検索し、キャンバスにドラッグ&amp;ドロップします。

   ![](assets/image2016-6-8-9-3a24-3a24.png)

   >[!NOTE]
   >
   >トリガーを使用したスマートキャンペーンは、トリガーモードで実行されます。 トリガーされたイベントと追加されたフィルターに基づいて、1 人につき一度ずつ実行されます。

1. ドロップダウンをクリックし、演算子を選択します。

   ![](assets/image2016-6-7-11-3a10-3a8.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーを示します。 修正されない場合、キャンペーンは無効になり、実行されません。

1. トリガーを定義します。

   ![](assets/image2016-6-7-11-3a12-3a23.png)

1. 必要に応じて、フィルターを追加します。

   ![](assets/image2016-6-7-11-3a14-3a20.png)

   >[!TIP]
   >
   >トリガーとフィルターの両方を含むスマートキャンペーンでは、トリガーが一番上に表示されます。 トリガーされると、フィルター条件を満たす人のみがフローを通過します。

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、いずれかのトリガーがアクティブ化すると、その人物はフローに進みます。

   一連のリードに対してキャンペーンを同時に実行するには、[スマートキャンペーンのスマートリストを定義する | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [予測コンテンツアクティビティのスマートリストの定義](/help/marketo/product-docs/predictive-content/define-a-smart-list-for-predictive-content-activities.md)
