---
unique-page-id: 1147027
description: 担当者をSFDCに同期 —Marketoドキュメント — 製品ドキュメント
title: 担当者を SFDC に同期
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 7%

---

# 担当者を SFDC に同期 {#sync-person-to-sfdc}

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

## 概要 {#overview}

このフローステップは、Marketoが作成した人々をリードとしてSalesforce CRMに挿入します。

![](assets/sync-person-to-sfdc.png)

## 使用状況 {#usage}

1. デフォルトでは、このフロー手順は、Salesforce自動割り当てルールに基づいて、リードの所有者に割り当てられます。

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Salesforceでは、会社と姓のフィールドに入力する必要があります。 それ以外の場合は、リードレコードが拒否されます。

1. 特定のSalesforceユーザーまたはリードキューをリード所有者として設定できます。

   ![](assets/sync-person-to-sfdc-2.png)

   このフローステップを使用する場合、担当者はSalesforceのリードとして即座に同期され、通常の同期を待つ必要はありません。

   >[!CAUTION]
   >
   >Salesforceでは、「連絡先」をリードキューに割り当てることはできません。 この場合、MarketoはSalesforceで重複「リード」を作成します。
