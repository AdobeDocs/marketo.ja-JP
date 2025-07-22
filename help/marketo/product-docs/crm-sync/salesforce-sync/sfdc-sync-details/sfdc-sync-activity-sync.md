---
unique-page-id: 2953473
description: SFDC同期 – アクティビティ同期 – Marketo ドキュメント – 製品ドキュメント
title: SFDC同期 – アクティビティ同期
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 71%

---

# SFDC 同期：アクティビティの同期 {#sfdc-sync-activity-sync}

Marketoは、[!DNL Salesforce] アクティビティデータも同期します。 質問と回答をいくつか示します。

## Marketo はどのタイプのアクティビティデータを同期しますか。 {#what-types-of-activity-data-does-marketo-sync-over}

Marketo は、リードまたは取引先責任者に関連付けられたイベントとタスクの両方を同期します。

## アクティビティの詳細は、2 つのシステム間でどのように同期されていますか。 {#how-are-activity-details-kept-in-sync-between-the-two-systems}

同期は、[!DNL Salesforce] からMarketoへの一方向です。 ただし、[!DNL Salesforce] タスクを作成 [ フローステップまたは ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) アクティビティ同期をカスタマイズ [ を使用して、](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md) でタスクを作成 [!DNL Salesforce] きます。

## Marketo を使用してタスクを作成することはできますか。 {#can-i-create-a-task-using-marketo}

はい。[タスクフローの作成アクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}を使用できます。

## アクティビティに関連するトリガー／フィルターには何がありますか。 {#what-are-the-triggers-filters-related-to-activity}

トリガー

* アクティビティの記録
* アクティビティの更新

フィルター

* アクティビティがログに記録されました／無操作状態が記録されました
* アクティビティは更新されました／無操作状態が更新されました

>[!TIP]
>
>「無操作状態」という言葉はわかりにくいですが、「無」は、無操作状態のフィルターを指します。詳しくは、[スマートリストでの無操作状態フィルターの使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}を参照してください。
