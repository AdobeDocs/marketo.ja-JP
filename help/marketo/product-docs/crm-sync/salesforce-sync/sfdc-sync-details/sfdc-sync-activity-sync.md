---
unique-page-id: 2953473
description: SalesforceのアクティビティとタスクをMarketoに同期する方法について説明します。 Marketoからタスクを作成し、スマートキャンペーンでアクティビティのトリガーとフィルターを使用します。
title: SFDC 同期 - アクティビティ同期
exl-id: 780e9cb7-b8b2-4a79-a0b8-d9d34a655330
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/N-pw1q0NXaJGKW1J1R4iqhgXhA42sX5nP0OWPXCuaBc'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 86%
---
# SFDC 同期：アクティビティ同期 {#sfdc-sync-activity-sync}

Marketo は、[!DNL Salesforce] アクティビティデータを介して同期も行います。 質問と回答をいくつか示します。

## Marketo はどのタイプのアクティビティデータを同期しますか。 {#what-types-of-activity-data-does-marketo-sync-over}

Marketo は、リードまたは取引先責任者に関連付けられたイベントとタスクの両方を同期します。

## アクティビティの詳細は、2 つのシステム間でどのように同期されていますか。 {#how-are-activity-details-kept-in-sync-between-the-two-systems}

同期は [!DNL Salesforce] から Marketo への一方向で行われます。 ただし、[タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)フローステップまたは[アクティビティの同期をカスタマイズ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync.md)を [!DNL Salesforce] に使用して、[!DNL Salesforce] でタスクを作成できます。

## Marketo を使用してタスクを作成することはできますか。 {#can-i-create-a-task-using-marketo}

はい。[タスクフローの作成アクション](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}を使用できます。

## アクティビティに関連するトリガー／フィルターには何がありますか。 {#what-are-the-triggers-filters-related-to-activity}

トリガー

* アクティビティの記録
* アクティビティの更新

フィルター

* アクティビティがログに記録されました／アクティビティがログに記録されていない
* アクティビティが更新されました／アクティビティが更新されていない

>[!TIP]
>
>「Not Activity」という表現がわかりにくいと感じるかもしれませんが、 ここでの「not」は、非アクティビティフィルター（Inactivity フィルター）を指します。 詳しくは、[スマートリストでの無操作状態フィルターの使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}を参照してください。
