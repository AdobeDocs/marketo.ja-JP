---
unique-page-id: 1147027
description: 個人を SFDC に同期する - Marketo ドキュメント - 製品ドキュメント
title: 個人を SFDC に同期する
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 41%

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
   >[!DNL Salesforce] では、人物の会社および姓フィールドが入力されている必要があります。 入力されていない場合、リードレコードは拒否されます。

1. 特定の [!DNL Salesforce] ユーザーまたはリードキューをリード所有者として設定できます。

   ![](assets/sync-person-to-sfdc-2.png)

   このフローステップを使用すると、その人物はすぐに [!DNL Salesforce] リードとして同期されるので、通常の同期を待つ必要はありません。

   >[!CAUTION]
   >
   >[!DNL Salesforce] では、「連絡先」をリードキューに割り当てることはできません。 この場合、Marketoは [!DNL Salesforce] で重複した「Lead」を作成します。
