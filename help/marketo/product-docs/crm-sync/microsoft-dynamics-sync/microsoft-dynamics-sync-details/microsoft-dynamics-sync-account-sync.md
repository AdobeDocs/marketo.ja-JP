---
unique-page-id: 3571836
description: Microsoft Dynamics Sync — アカウント同期 — Marketto Docs — 製品ドキュメント
title: Microsoft Dynamics Sync — アカウントの同期
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics同期：アカウントの同期{#microsoft-dynamics-sync-account-sync}

Marketoがデータベース全体をDynamicsと同期することを知っていますか。 同期して5分待ち、その後、毎日、再び同期します。 MarketoがDynamicsアカウントを具体的に扱う方法について、いくつかの詳細を示します。

## 情報の同期方法{#which-way-does-the-information-sync}

次の1つの方法のみ：DynamicsからMarketoへ

## アップデートの動作{#how-do-the-updates-work}

Marketorの担当者の「アカウント」フィールドを更新すると、Marketorのそのアカウントに属するすべての担当者の値が変更されます。 Dynamicsと同期されません。 ただし、次回Dynamicsでアカウントが更新されたときは、Marketorのすべてのアカウント情報が変更によって上書きされます。

## Marketoを使用してアカウントを作成できますか。{#can-i-create-an-account-using-marketo}

いいえ。 Marketing CloudのアカウントをDynamicsで作成できません。

## Marketoと同期するフィールドはどれか。{#which-fields-will-sync-to-marketo}

[設定中に、同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)できます。 ただし、Dynamics同期ユーザーがアクセス権を持つフィールドのみが同期されます。

## Dynamicsの[アカウント]フィールドを変更すると、各連絡先の[データ値の変更]アクティビティログが生成されますか。 {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

ほとんどはそうです。 ただし、アカウントに5,000個を超える連絡先があり、そのアカウントのフィールドがDynamicsで変更された場合は、変更を同期しますが、5,000個を超える連絡先のアクティビティは記録されません。
