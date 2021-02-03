---
unique-page-id: 2953473
description: SFDC同期 —アクティビティ同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 —アクティビティ同期
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# SFDC同期：アクティビティ同期{#sfdc-sync-activity-sync}

また、MarketoはSalesforceアクティビティデータを同期します。 質問と回答をいくつか示します。

## Marketorはどのようなタイプのアクティビティデータを同期しますか。{#what-types-of-activity-data-does-marketo-sync-over}

マーケティング担当者は、リードまたは担当者に関連付けられたイベントとタスクの両方で同期します。

## 2つのシステム間でアクティビティの詳細を同期させる方法{#how-are-activity-details-kept-in-sync-between-the-two-systems}

同期は、SalesforceからMarketoへの1つの方法です。 ただし、[タスクの作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)フローステップまたは[アクティビティのカスタマイズ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md)を使用して、Salesforceでタスクを作成できます。

## Marketoを使用してタスクを作成できますか。{#can-i-create-a-task-using-marketo}

はい、[タスクフローの作成アクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)を使用できます。

## アクティビティに関連するトリガー/フィルターは何か。{#what-are-the-triggers-filters-related-to-activity}

トリガー

* アクティビティがログに記録される
* アクティビティが更新されました

フィルター

* アクティビティがログに記録されたか、アクティビティがログに記録されませんでした
* アクティビティが更新された/アクティビティが更新されませんでした

>[!TIP]
>
>「アクティビティでない」という言葉が分からない場合は、 「not」は、無操作状態フィルタを指します。 詳しくは、次を参照してください。[スマートリストで無操作フィルターを使用する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)
