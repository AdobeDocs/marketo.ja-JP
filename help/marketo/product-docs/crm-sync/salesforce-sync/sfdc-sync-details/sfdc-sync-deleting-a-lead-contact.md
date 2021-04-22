---
unique-page-id: 7515131
description: SFDC同期 — リード/連絡先の削除 —Marketoドキュメント — 製品ドキュメント
title: SFDCの同期 — リード/連絡先の削除
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# SFDC同期：リード/連絡先の削除{#sfdc-sync-deleting-a-lead-contact}

以下に、詳細を示します。

* Marketoは、Salesforceでリードが削除されたので、自動的に人を削除しません。 「SFDC Is Deleted」フラグがtrueに設定されている場合は、 必要に応じて、このフィールドをトリガーオフにして、Marketoで削除できます。
* [「](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) パーソンフローの削除」アクション。MKTO内の人物を削除しますが、`Salesforce`内でも削除する選択肢があります。

* [SFDCflowから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) アクション：これによりSFDCのリードは削除されますが、Marketoの人物も削除できます。
* Salesforceでリードを削除し(ただし、個人がMarketoで削除されていない場合)、その後[Salesforce](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)と同期フローアクションを実行すると、Salesforceで新しいリードが作成されます。
