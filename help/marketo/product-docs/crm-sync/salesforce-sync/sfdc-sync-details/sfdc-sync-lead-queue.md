---
unique-page-id: 7516241
description: SFDC同期 — リードキュー — マーケティング担当者向けドキュメント — 製品ドキュメント
title: SFDC同期 — リードキュー
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# SFDC同期：リードキュー{#sfdc-sync-lead-queue}

Marketorでは、顧客を[Salesforceのリードキュー](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm)に追加して、リードの配信に役立てることができます。 詳しくは、

## Marketorのキューに人を割り当てる方法{#how-to-assign-a-person-to-a-queue-in-marketo}

次のいずれかのフロー処理を使用して、Salesforceのリードキューに個人を割り当てることができます。

* [担当者をSFDCに同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [所有者の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Marketoのキューを作成したり変更したりすることはできません。

## 個人がキューに属している場合、リードの所有者情報はどのように保存されますか。{#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

リードがSalesforceのキューに所有されている場合、リードが所有者に割り当てられるまで、これらの販売所有者フィールドは空のままです。

* 販売所有者の名
* 販売所有者の姓
* 販売所有者の役職
* 販売所有者の電話番号
* 販売所有者の電子メールアドレス
