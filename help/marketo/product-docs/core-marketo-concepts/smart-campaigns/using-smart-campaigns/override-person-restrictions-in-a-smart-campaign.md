---
unique-page-id: 1147066
description: スマートキャンペーンでのリード制限数の上書き - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーンでのリード制限数の上書き
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 35%

---

# スマートキャンペーンでのリード制限数の上書き {#override-person-restrictions-in-a-smart-campaign}

Marketo Engageを使用すると、スマートキャンペーンの対象となる最大人数を設定できます。これにより、データベース全体に誤ってメールが送信されるのを回避できます。 この制限を&#x200B;_上書き_&#x200B;する場合は、次の手順に従います。

>[!PREREQUISITES]
>
>Marketo管理で [ スマートキャンペーンの人物制限を有効にする ](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} を必ずオンにします。

1. **[!UICONTROL マーケティングアクティビティ]** で、スマートキャンペーンに移動し、「**[!UICONTROL スケジュール]**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. スマートキャンペーン設定で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >デフォルトの制限は、管理で設定された制限です。

1. 新しい制限を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   対象となるユーザーの数が設定された制限を超えた場合、スマートキャンペーンは実行されません。

   >[!CAUTION]
   >
   >この機能を使用する場合は、誤って多くの人を含めないようにご注意ください。
