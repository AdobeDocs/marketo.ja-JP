---
unique-page-id: 7515131
description: SFDC 同期 - リード／取引先責任者の削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード／取引先責任者の削除
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 83%

---

# SFDC 同期：リード／取引先責任者の削除 {#sfdc-sync-deleting-a-lead-contact}

以下に詳細を示します。

* Marketo Engageは、リードが Salesforce で削除されたので、担当者を自動的に削除しません。 代わりに、「SFDC Is Deleted」フラグが true に設定されます。 必要に応じて、このフィールドをトリガーにして、Marketo で削除できます。
* [顧客の削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md){target="_blank"}フローアクション。これは、MKTO で人物を削除するものですが、`Salesforce` で削除することも選択できます。

* [SFDC から削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md){target="_blank"}フローアクション：これは、SFDC  でリードを削除するものですが、Marketo で人物を削除することも選択できます。
* リードが Salesforce で削除され（Marketo では人物は削除されない）、その後、[Salesforce との同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}フローアクションを実行すると、Salesforce で新しいリードが作成されます。
