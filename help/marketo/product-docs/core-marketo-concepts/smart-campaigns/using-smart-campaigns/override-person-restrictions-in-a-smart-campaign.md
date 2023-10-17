---
unique-page-id: 1147066
description: スマートキャンペーンでのリード制限数の上書き - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーンでのリード制限数の上書き
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: fec5219c599c805328d77797d2636e549e489ca5
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 46%

---

# スマートキャンペーンでのリード制限数の上書き {#override-person-restrictions-in-a-smart-campaign}

Marketo Engageを使用すると、スマートキャンペーンの対象として認定できる最大人数を設定できます。これにより、データベース全体に誤って電子メールが送信されるのを防ぐことができます。 この制限を&#x200B;_上書き_&#x200B;する場合は、次の手順に従います。

>[!PREREQUISITES]
>
>必ず [スマートキャンペーンの担当者制限の有効化](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} Marketo Admin の

1. マーケティングアクティビティで、スマートキャンペーンに移動し、 **スケジュール**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. スマートキャンペーン設定で、「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >デフォルトの制限は、管理で設定された制限です。

1. 新しい制限を入力し、 **[!UICONTROL 保存]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   認定された担当者の数が設定された制限を超えると、スマートキャンペーンは実行されません。

   >[!CAUTION]
   >
   >誤って多くのリードを含めすぎないように、この機能を活用してください。
