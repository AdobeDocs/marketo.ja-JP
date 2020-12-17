---
unique-page-id: 7515131
description: SFDCの同期 — リード/連絡先の削除 — Marketto Docs — 製品ドキュメント
title: SFDCの同期 — リード/連絡先の削除
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# SFDC同期：リード/連絡先の削除{#sfdc-sync-deleting-a-lead-contact}

以下に、詳細を示します。

* Salesforceでリードが削除されたので、Marketorはユーザーを自動的に削除しません。 「SFDC Is Deleted」フラグがtrueに設定されている場合は、 必要に応じて、Marketorでこのフィールドをトリガーして削除できます。
* [「](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) パーソンフローの削除」アクション。MKTO内の人物を削除しますが、`Salesforce`内でも削除する選択肢があります。

* [SFDCflowから削除](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) アクション：これによりSFDCのリードは削除されますが、マーケティング担当者を削除することもできます。
* リードがSalesforceで削除された（ただし、Marketoでは削除されなかった）場合、その後[Salesforceと同期](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)のフロー操作を実行すると、Salesforceで新しいリードが作成されます。

つまり魔法のように動く！

![—](assets/image2015-5-20-15-3a3-3a27.png)

