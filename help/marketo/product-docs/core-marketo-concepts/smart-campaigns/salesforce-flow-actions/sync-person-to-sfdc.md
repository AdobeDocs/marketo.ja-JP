---
unique-page-id: 1147027
description: フローステップを使用して人物をSalesforceに同期する方法について説明します。 フローに参加したリードまたは連絡先のデータをSFDCにプッシュします。
title: 個人を SFDC に同期する
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/jU7Hg1x8TUfxR4GnO1oxvJXh-8X3LVXll9z8k5Eck80
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 143
ht-degree: 83%

---

# 個人を SFDC に同期する {#sync-person-to-sfdc}

このフローステップは、Marketo が作成した人物を Salesforce CRM に挿入するものです。

>[!NOTE]
>
>[!DNL Salesforce] と統合されている場合にのみ使用できます。

1. デフォルトでは、このフローステップは、Salesforce 自動割り当てルールに基づいてリード所有者に割り当てます。

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] では、人物の「会社」と「姓」のフィールドが入力されている必要があります。 入力されていない場合、リードレコードは拒否されます。

1. 特定の [!DNL Salesforce] ユーザまたはリードのキューをリード所有者として設定できます。

   ![](assets/sync-person-to-sfdc-2.png)

   このフローステップを使用する場合、人物は [!DNL Salesforce] のリードとして即座に同期され、通常の同期を待つ必要はありません。

   >[!CAUTION]
   >
   >[!DNL Salesforce] では「取引先責任者」をリードのキューに割り当てることはできません。 この場合、Marketo は [!DNL Salesforce] で「リード」を重複して作成します。
