---
unique-page-id: 3571836
description: Microsoft Dynamics Sync — アカウントの同期 — Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics Sync — アカウントの同期
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 100%

---

# Microsoft Dynamics Sync:アカウントの同期 {#microsoft-dynamics-sync-account-sync}

Marketoがデータベース全体をDynamicsと同期しているのを知っていましたか？ 同期し、5分待ってから、毎日、再び同期します。 MarketoでのDynamicsアカウントの処理方法の詳細を以下に示します。

## 情報の同期方法 {#which-way-does-the-information-sync}

1つの方法のみ：DynamicsからMarketo

## 更新の仕組み {#how-do-the-updates-work}

Marketoで連絡先の「アカウント」フィールドを更新すると、Marketoでそのアカウントに属するすべての連絡先の値が変更されます。 Dynamicsとは同期しません。 ただし、次回Dynamicsでそのアカウントが更新されたときは、Marketoのすべてのアカウント情報が変更によって上書きされます。

## Marketoを使用してアカウントを作成できますか？ {#can-i-create-an-account-using-marketo}

いいえ. MarketoはDynamicsにアカウントを作成できません。

## Marketoと同期するフィールドは何ですか。 {#which-fields-will-sync-to-marketo}

[設定時に同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。 ただし、Marketoは、Dynamics同期ユーザーがアクセスできるフィールドのみを同期します。

## Dynamicsの「アカウント」フィールドに変更を加えると、各連絡先の「データ値の変更」アクティビティログが生成されますか？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

主には、はい。 ただし、アカウントに5,000件を超える連絡先があり、そのアカウントのフィールドがDynamicsで変更された場合は、変更を同期しますが、5,000件以上の連絡先のアクティビティはログに記録されません。
