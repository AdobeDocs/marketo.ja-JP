---
unique-page-id: 7515131
description: SFDC 同期 - リード／取引先責任者の削除 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード／取引先責任者の削除
exl-id: b859357e-09c5-48e5-940e-f5b4e955e374
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 100%

---

# SFDC 同期：リード／取引先責任者の削除 {#sfdc-sync-deleting-a-lead-contact}

以下に詳細を示します。

* [!DNL Salesforce] でリードが削除された場合でも、Marketo が自動的に人物を削除することはありません。代わりに、フィールドの「SFDC 削除済み」フラグが true に設定されます。必要に応じて、このフィールドをトリガーにして、Marketo で削除できます。
* [顧客の削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md)フローアクション。これは、MKTO で人物を削除するものですが、`Salesforce` で削除することも選択できます。

* [SFDC から削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md)フローアクション：これは、SFDC  でリードを削除するものですが、Marketo で人物を削除することも選択できます。
* リードが [!DNL Salesforce] で削除され（Marketo では人物は削除されない）、その後、[ [!DNL Salesforce]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) との同期フローアクションを実行すると、[!DNL Salesforce] で新しいリードが作成されます。
