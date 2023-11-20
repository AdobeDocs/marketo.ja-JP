---
unique-page-id: 2953455
description: SFDC 同期 - リードの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リードの同期
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 95%

---

# SFDC 同期：リードの同期 {#sfdc-sync-lead-sync}

Salesforce データベースのMarketo Engage同期をご存知でしたか？ 同期して 5 分待機し、その後また同期するという処理を一日中、毎日繰り返しおこなっています。Marketo による Salesforce リードの処理方法の詳細を以下に示します。

## 同期の方向 {#sync-direction}

リード（顧客）とコンタクトの同期は双方向です。Salesforce または Marketo の取引先責任者に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo が優先されます。このようなデータの競合が発生することは、ほとんどありません。

## Marketo を使用して Salesforce でリードを作成することはできますか。 {#can-i-create-a-lead-in-salesforce-using-marketo}

はい、「[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}」フローアクションを使用します。リードが存在しない場合、Salesforce にリードが作成されます。

## Marketo の顧客を手動で Salesforce のリードと同期させることはできますか。 {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketo は、Salesforce 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketo は Salesforce の検証ルールを遵守しますか。 {#will-marketo-respect-the-salesforce-validation-rules}

はい。データ形式が正しくない場合や、必須フィールドの情報が見つからない場合は、同期が失敗します。この場合、Marketo はリードのアクティビティログに結果を記録します。
