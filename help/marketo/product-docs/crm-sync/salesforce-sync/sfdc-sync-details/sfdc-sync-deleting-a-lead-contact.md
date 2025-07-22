---
unique-page-id: 7515131
description: SFDC 同期 - リード／取引先責任者の削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード／取引先責任者の削除
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 68%

---

# SFDC 同期：リード／取引先責任者の削除 {#sfdc-sync-deleting-a-lead-contact}

以下に詳細を示します。

* リードが [!DNL Salesforce] で削除されたからといって、Marketoによってユーザーが自動的に削除されるわけではありません。 代わりに、フィールドの「SFDC 削除済み」フラグが true に設定されます。必要に応じて、このフィールドをトリガーにして、Marketo で削除できます。
* [顧客の削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md)フローアクション。これは、MKTO で人物を削除するものですが、`Salesforce` で削除することも選択できます。

* [SFDC から削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md)フローアクション：これは、SFDC  でリードを削除するものですが、Marketo で人物を削除することも選択できます。
* [!DNL Salesforce] でリードが削除され（ただし、Marketoでは個人は削除されません）、その後 [ 次と同期  [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) フローアクションが実行された場合、[!DNL Salesforce] で新しいリードが作成されます。
