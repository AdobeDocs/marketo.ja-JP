---
unique-page-id: 1147021
description: 所有者の変更 - Marketo ドキュメント - 製品ドキュメント
title: 所有者の変更
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 80%

---

# 所有者の変更 {#change-owner}

このフローステップを使用して、既に所有者に割り当てられている人物を別の所有者に再割り当てできます。

![](assets/change-owner-1.png)

1. 変更したい所有者もしくはリードのキューを選択します。

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >[!DNL Salesforce] では、連絡先をリードキューに割り当てることはできません。 SFDC 取引先責任者のレコードの場合：
   >
   >* Marketo は、取引先責任者が Salesforce に同期された&#x200B;**場合のみ**、リードを重複して作成します。つまり、**[リードを SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;フローステップを `AssignTo=<a lead queue>` と共に使用すると、Marketo は Salesforce で重複したリードを作成し、リードキューに割り当てます。
   >
   >* 取引先責任者に&#x200B;**[!UICONTROL 所有者を変更]**&#x200B;フローステップを使用すると、Marketo は Salesforce に重複したリードを作成します。この問題を回避するには、「SFDC タイプ」フィールドで、アクションをリードのみに制限するフィルターを使用します。

   >[!NOTE]
   >
   >[!DNL Salesforce] アカウントにまだレコードが存在しない場合、同期が行われ、選択したユーザーに割り当てられます。
