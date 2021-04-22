---
unique-page-id: 7516241
description: SFDC同期 — リードキュー —Marketoドキュメント — 製品ドキュメント
title: SFDC同期 — リードキュー
exl-id: b3b5e14c-f914-429c-a4b9-6b535ad8e882
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 15%

---

# SFDC同期：リードキュー{#sfdc-sync-lead-queue}

Marketoでは、[Salesforceのリードキュー](https://help.salesforce.com/apex/HTViewHelpDoc?id=queues_overview.htm)に人を追加して、リードの配信に役立てることができます。 詳しくは、

## Marketoのキューに人を割り当てる方法{#how-to-assign-a-person-to-a-queue-in-marketo}

次のいずれかのフロー処理を使用して、Salesforceのリードキューに個人を割り当てることができます。

* [担当者を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)
* [所有者の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)

>[!NOTE]
>
>Marketoではキューを作成したり変更したりできません。

## 個人がキューに属している場合、リードの所有者情報はどのように保存されますか。{#how-is-lead-owner-information-stored-if-the-person-belongs-to-a-queue}

リードがSalesforceのキューに所有されている場合、リードが所有者に割り当てられるまで、これらの販売所有者フィールドは空のままです。

* セールス所有者の名
* セールス所有者の姓
* 販売所有者の役職
* セールス所有者の電話番号
* セールス所有者のメールアドレス
