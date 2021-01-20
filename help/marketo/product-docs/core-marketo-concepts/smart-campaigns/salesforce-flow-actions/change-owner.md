---
unique-page-id: 1147021
description: 所有者の変更 — Marketto Docs — 製品ドキュメント
title: 所有者の変更
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# 所有者の変更{#change-owner}

既に所有者に割り当てられている既存のユーザーがある場合は、このフロー手順を使用して別の所有者に再割り当てできます。

![](assets/image2014-9-22-15-3a1-3a3.png)

**使用状況**

1. 変更する所有者またはリードキューを選択して移動します。

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforceでは、連絡先をリードキューに割り当てることはできません。 SFDCの担当者であるレコードの場合：
   >
   >1. Marketorは、連絡先がSalesforceと同期された場合に、重複リード&#x200B;**のみ**&#x200B;を作成します。 つまり、**[「個人をSFDCに同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**」のフローステップを`AssignTo=<a lead queue>`と共に使用する場合、MarketoはSalesforceで重複リードを作成し、それをリードキューに割り当てます。
      >
      >
   1. 連絡先に対して&#x200B;**所有者の変更**&#x200B;フローステップを使用しようとすると、Salesforceに重複は作成されません。


   >[!NOTE]
   >
   >Salesforceアカウントにレコードがまだ存在しない場合は、同期し、選択したユーザーに割り当てます。
