---
unique-page-id: 2953455
description: SFDC 同期 - リード同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード同期
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '237'
ht-degree: 100%

---

# SFDC 同期：リード同期 {#sfdc-sync-lead-sync}

Marketo が Salesforce とデータベースを同期していることをご存じでしょうか。同期して 5 分待機し、その後また同期するという処理を一日中、毎日繰り返しおこなっています。Marketo による Salesforce リードの処理方法の詳細を以下に示します。

## 同期方向 {#sync-direction}

リード（顧客）とコンタクトの同期は双方向です。Salesforce または Marketo の取引先責任者に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo が優先されます。この種のデータの衝突はめったに起こりません。

## Marketo を使用して Salesforce でリードを作成することはできますか。 {#can-i-create-a-lead-in-salesforce-using-marketo}

はい、「[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)」フローアクションを使用します。リードが存在しない場合、Salesforce にリードが作成されます。

## Marketo の顧客を手動で Salesforce のリードと同期させることはできますか。 {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

はい、「[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)」フローアクションを使用すると、リアルタイムで同期されます。

## すべての標準フィールドが Marketo と同期されますか。 {#does-every-single-standard-field-sync-to-marketo}

いいえ。標準フィールドには同期できないものもあります。カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketo は、Salesforce 同期ユーザーがアクセスできるフィールドのみを同期します。

## Marketo は Salesforce の検証ルールを遵守しますか。 {#will-marketo-respect-the-salesforce-validation-rules}

はい。データ形式が正しくない場合や、必須フィールドの情報が見つからない場合は、同期が失敗します。この場合、Marketo はリードのアクティビティログに結果を記録します。
