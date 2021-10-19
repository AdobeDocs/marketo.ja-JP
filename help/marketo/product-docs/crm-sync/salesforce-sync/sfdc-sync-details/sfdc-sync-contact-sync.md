---
unique-page-id: 2953457
description: SFDC 同期 - 連絡先の同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - 連絡先の同期
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '235'
ht-degree: 100%

---

# SFDC 同期：連絡先の同期 {#sfdc-sync-contact-sync}

Marketo は、データベース全体を Salesforce と同期しています。同期した後、5 分待ってからまた同期するということを、1 日中、毎日繰り返しています。ここでは、Marketo が Salesforce の連絡先をどのように扱っているかを詳しく説明します。

## 同期の方向 {#sync-direction}

連絡先の同期は、双方向です。Salesforce または Marketo で連絡先に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで同時に変更が加えられた場合の動作 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Salesforce での変更を優先します。このようなデータの競合が発生することは、ほとんどありません。

## 人物の Marketo の連絡先への変換 {#can-i-convert-a-person-into-a-contact-in-marketo}

**[顧客を変換](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**&#x200B;フローアクションを使用することで実現できます。

>[!CAUTION]
>
>Marketo で人物を変換すると、Salesforce で新しいアカウントと商談が作成されます。アカウントを重複させたくない場合は、Salesforce を使用して変換します。

## 手動での連絡先の同期の強制 {#can-i-manually-force-a-sync-of-a-contact}

**[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。すべてのカスタムフィールドを同期することはできます。

>[!NOTE]
>
>Marketo は、Marketo 同期ユーザーがアクセスできるフィールドのみを同期します。

## Marketo による Salesforce の検証ルールの尊重 {#will-marketo-respect-the-salesforce-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
