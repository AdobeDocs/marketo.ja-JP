---
unique-page-id: 1147025
description: スマートキャンペーンでWebhookを使用する方法を説明します。 外部URLを呼び出し、フローステップから人物データを渡します。
title: スマートキャンペーンでの web フックの使用
exl-id: 19dcc469-288d-4bfb-92e1-3e8db75588a6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/8eKQKnmuizYtT926nDvDBHWBLDmUV3lZQYCfezuviEg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 127
ht-degree: 82%

---

# スマートキャンペーンでの web フックの使用 {#use-a-webhook-in-a-smart-campaign}

[Web フック](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/webhooks/webhooks){target="_blank"}を使用するには、フローアクションとして[スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}に追加します。

>[!AVAILABILITY]
>
>すべての Marketo Engage ユーザがこの機能を購入しているわけではありません。 詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

1. [スマートキャンペーンを作成します](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}。

   >[!NOTE]
   >
   >Web フックは、トリガーキャンペーンでのみ使用できます。

1. 「**[!UICONTROL フロー]**」タブに移動し、「**[!UICONTROL Web フックを呼び出し]**」フローアクションをドラッグします。

   ![](assets/use-a-webhook-in-a-smart-campaign-1.png)

1. 「**[!UICONTROL Web フック]**」を選択します。

   ![](assets/use-a-webhook-in-a-smart-campaign-2.png)

1. スマートリストでも web フックを使用できます。

   ![](assets/use-a-webhook-in-a-smart-campaign-3.png)

1. 最後に、フローステップの「**[!UICONTROL 選択肢を追加]**」で web フックを使用できるようになります。

   ![](assets/use-a-webhook-in-a-smart-campaign-4.png)
