---
unique-page-id: 3571836
description: Microsoft Dynamics Sync — アカウントの同期 — Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics Sync — アカウントの同期
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 42%

---

# [!DNL Microsoft Dynamics] 同期：アカウント同期 {#microsoft-dynamics-sync-account-sync}

Marketoがデータベース全体を [!DNL Dynamics] と同期することをご存知ですか？ 同期し、5分待ってから、毎日、再び同期します。Marketoにおける [!DNL Dynamics] アカウントの具体的な取り扱い方法について詳しくは、以下を参照してください。

## 情報の同期方向 {#which-way-does-the-information-sync}

唯一の方法：[!DNL Dynamics] からMarketoへ。

## 更新の仕組み {#how-do-the-updates-work}

Marketo で取引先責任者の「アカウント」フィールドを更新すると、Marketo でそのアカウントに属するすべての取引先責任者の値が変更されます。[!DNL Dynamics] とは同期されません。 ただし、そのアカウントが次回 [!DNL Dynamics] で更新されると、その変更はMarketoのすべてのアカウント情報を上書きします。

## Marketoを使用してアカウントを作成できますか？ {#can-i-create-an-account-using-marketo}

いいえ.Marketoは、[!DNL Dynamics] でアカウントを作成できません。

## Marketoと同期するフィールドは何ですか。 {#which-fields-will-sync-to-marketo}

[設定時に同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync)できます。ただし、Marketoで同期されるのは、[!DNL Dynamics] sync ユーザーがアクセスできるフィールドのみです。

## [!DNL Dynamics] のアカウントフィールドを変更すると、各連絡先の「データ値を変更」アクティビティログが表示されますか？  {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

主には、はい。ただし、アカウントに 5,000 を超える連絡先があり、そのアカウントのフィールドが [!DNL Dynamics] で変更された場合、変更を同期しますが、5,000 を超える連絡先のアクティビティはログに記録されません。
