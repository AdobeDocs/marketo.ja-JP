---
unique-page-id: 2953457
description: SFDC 同期 - 取引先責任者の同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - 取引先責任者の同期
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: ht
source-wordcount: '235'
ht-degree: 100%

---

# SFDC 同期：取引先責任者の同期 {#sfdc-sync-contact-sync}

Marketo は、データベース全体を Salesforce と同期しています。同期した後、5 分待ってからまた同期するということを、1 日中、毎日繰り返しています。ここでは、Marketo が Salesforce の取引先責任者をどのように扱っているかを詳しく説明します。

## 同期の方向 {#sync-direction}

取引先責任者の同期は、双方向です。Salesforce または Marketo で取引先責任者に変更を加えると、更新内容が両方のシステムに反映されます。

## 両方のシステムで変更が同時に行われた場合はどうなりますか。 {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Salesforce での変更を優先します。このようなデータの競合が発生することは、ほとんどありません。

## 人物の Marketo の取引先責任者への変換 {#can-i-convert-a-person-into-a-contact-in-marketo}

**[顧客を変換](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**&#x200B;フローアクションを使用することで実現できます。

>[!CAUTION]
>
>Marketo で人物を変換すると、Salesforce で新しいアカウントと商談が作成されます。アカウントを重複させたくない場合は、Salesforce を使用して変換します。

## 手動での取引先責任者の同期の強制 {#can-i-manually-force-a-sync-of-a-contact}

**[顧客を SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)**&#x200B;フローアクションを使用して、リアルタイムで同期できます。

## すべての標準フィールドの Marketo への同期 {#does-every-single-standard-field-sync-to-marketo}

すべての標準フィールドが有用というわけではなく、すべて同期されるわけではありません。カスタムフィールドはすべて同期に含めることができます。

>[!NOTE]
>
>Marketo は、Marketo 同期ユーザがアクセスできるフィールドのみを同期します。

## Marketo は Salesforce の検証ルールを遵守しますか。 {#will-marketo-respect-the-salesforce-validation-rules}

検証ルールが尊重され、競合が発生した場合、結果がリードのアクティビティログに記録されます。
