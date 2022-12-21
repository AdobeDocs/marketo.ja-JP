---
unique-page-id: 2953459
description: SFDC の同期 - アカウントの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC の同期 - アカウントの同期
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 100%

---

# SFDC 同期：アカウントの同期 {#sfdc-sync-account-sync}

Marketo は、アカウント情報を Salesforce と同期します。次に、知っておくべき点をいくつか示します。

## 情報の同期方向 {#which-way-does-the-information-sync}

同期は SFDC から Marketo への一方向です。

## 更新の仕組み {#how-do-the-updates-work}

Marketo で取引先責任者の「アカウント」フィールドを更新すると、Marketo でそのアカウントに属するすべての取引先責任者の値が変更されます。SFDC とは同期しません。ただし、次回 SFDC でアカウントが更新されたときは、Marketo のすべてのアカウント情報が変更によって上書きされます。

## 1 人の取引先責任者が複数のアカウントに属することはできますか？  {#can-a-contact-belong-to-multiple-accounts}

いいえ。1 つのアカウントには、複数の取引先責任者を含めることができます。1 つの取引先責任者には、1 つのアカウントのみを含めることができます。

## Marketo からアカウントを作成できますか？ {#can-i-create-accounts-from-marketo}

ほとんどできません。ただし、個人に対して[個人をコンバージョンする](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)フローステップを使用すると、新しい取引先責任者、新しいアカウント、新しい商談が作成されます。

>[!CAUTION]
>
>このフローステップの使用例は非常に限られています。確かでないなら、使わない方がいいです。

## Salesforce の「アカウント」フィールドに変更を加えると、各取引先責任者の「データ値の変更」アクティビティログが表示されますか。  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

ほとんどの場合されます。ただし、アカウントに 5,000 人を超える取引先責任者が存在し、そのアカウントのフィールドが SFDC で変更された場合は、変更を同期しますが、5,000 人を超える取引先責任者のアクティビティはログに記録されません。
