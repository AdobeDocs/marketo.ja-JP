---
unique-page-id: 7515131
description: SFDCの同期 — リード/連絡先の削除 — Marketto Docs — 製品ドキュメント
title: SFDCの同期 — リード/連絡先の削除
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---


# SFDC同期：リード/連絡先の削除{#sfdc-sync-deleting-a-lead-contact}

以下に、詳細を示します。

* Salesforceでリードが削除されたので、Marketorはユーザーを自動的に削除しません。 「SFDC Is Deleted」フラグがtrueに設定されている場合は、 必要に応じて、このフィールドをトリガーして、マーケティング担当者内で削除できます。
* [「](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) パーソンフローの削除」アクション。MKTO内の人物を削除しますが、`Salesforce`内でも削除する選択肢があります。

* [SFDCflowから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) アクション：これによりSFDCのリードは削除されますが、マーケティング担当者を削除することもできます。
* リードがSalesforceで削除された（ただし、Marketoでは削除されなかった）場合、その後[Salesforceと同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)のフロー操作を実行すると、Salesforceで新しいリードが作成されます。
