---
unique-page-id: 1147027
description: 担当者をSFDCに同期 — マーケティング担当者ドキュメント — 製品ドキュメント
title: 担当者をSFDCに同期
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# 担当者をSFDCに同期 {#sync-person-to-sfdc}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

## 概要 {#overview}

このフローステップは、Marketoが作成した人をSalesforce CRMへのリードとして挿入します。

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
   >Salesforceでは、「連絡先」をリードキューに割り当てることはできません。 この場合、MarketorはSalesforceに「リード」という重複を作成します。

