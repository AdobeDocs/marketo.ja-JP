---
unique-page-id: 1147027
description: 担当者をSFDCに同期 — マーケティング担当者ドキュメント — 製品ドキュメント
title: 担当者をSFDCに同期
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 0%

---


# 担当者をSFDCに同期{#sync-person-to-sfdc}

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

## 概要{#overview}

このフローステップは、Marketoが作成した人をSalesforce CRMへのリードとして挿入します。

![](assets/sync-person-to-sfdc.png)

## 使用法{#usage}

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
   >Salesforceでは、「連絡先」をリードキューに割り当てることはできません。 この場合、MarketorはSalesforceに「リード」という重複を作成します。
