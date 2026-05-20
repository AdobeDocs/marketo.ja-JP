---
unique-page-id: 1147066
description: スマートキャンペーンでユーザーの制限を上書きする方法を説明します。 通信制限に達した場合でも実行できるようにします。
title: スマートキャンペーンでのリード制限数の上書き
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 26%

---

# スマートキャンペーンでのリード制限数の上書き {#override-person-restrictions-in-a-smart-campaign}

Marketo Engageでは、スマートキャンペーンの対象となる最大人数を設定できます。これにより、データベース全体に誤ってメールを送信するのを防ぐことができます。 この制限を&#x200B;_上書き_&#x200B;する場合は、次の手順に従います。

>[!PREREQUISITES]
>
>Marketo Adminで[&#x200B; スマートキャンペーンのユーザー制限を有効にする](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"}必要があります。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;で、スマートキャンペーンに移動し、**[!UICONTROL スケジュール]**&#x200B;をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. スマートキャンペーン設定で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >デフォルトの制限は、管理で設定された制限です。

1. 新しい制限を入力し、**[!UICONTROL 保存]**&#x200B;をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   条件を満たす人数が設定された制限を超えた場合、スマートキャンペーンは実行されません。

   >[!CAUTION]
   >
   >誤って多くの人を含めないように、この機能に注意してください。
