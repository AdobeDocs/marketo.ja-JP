---
unique-page-id: 2953455
description: SFDC 同期 - リードの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リードの同期
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 100%

---

# SFDC 同期：リードの同期 {#sfdc-sync-lead-sync}

Marketo が [!DNL Salesforce] データベースと同期していることを知っていましたか？同期して 5 分待機し、その後また同期するという処理を一日中、毎日繰り返しおこなっています。ここでは、Marketo が [!DNL Salesforce] のリードをどのように扱っているかを詳しく説明します。

## 同期の方向 {#sync-direction}

リード（顧客）とコンタクトの同期は双方向です。[!DNL Salesforce] または Marketo のレコードに変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo が優先されます。このようなデータの競合が発生することは、ほとんどありません。

## Marketo を使用して [!DNL Salesforce] でリードを作成することはできますか？ {#can-i-create-a-lead-in-salesforce-using-marketo}

はい、「[人物を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)」フローアクションを使用します。リードが存在しない場合、[!DNL Salesforce] にリードが作成されます。

## Marketo の人物を手動で [!DNL Salesforce] のリードと同期させることはできますか？ {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketoは、[!DNL Salesforce] 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketo は [!DNL Salesforce] の検証ルールを遵守しますか？ {#will-marketo-respect-the-salesforce-validation-rules}

はい。データ形式が正しくない場合や、必須フィールドの情報が見つからない場合は、同期が失敗します。この場合、Marketo はリードのアクティビティログに結果を記録します。
