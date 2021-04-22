---
unique-page-id: 3571836
description: Microsoft Dynamics Sync — アカウント同期 —Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics Sync — アカウントの同期
exl-id: 86249d33-60dd-47e1-a7c8-3996c9444084
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# Microsoft Dynamics同期：アカウントの同期{#microsoft-dynamics-sync-account-sync}

Marketoがデータベース全体をDynamicsと同期するのを知っていましたか？ 同期して5分待ち、その後、毎日、再び同期します。 ここでは、MarketoがDynamicsアカウントを具体的に扱う方法について説明します。

## 情報の同期方法{#which-way-does-the-information-sync}

次の1つの方法のみ：ダイナミクスからMarketoまで

## アップデートの動作{#how-do-the-updates-work}

Marketoの連絡先の[アカウント]フィールドを更新すると、Marketoのそのアカウントに属するすべての連絡先の値が変更されます。 Dynamicsと同期されません。 ただし、次回Dynamicsでアカウントが更新されたときは、この変更により、Marketoのすべてのアカウント情報が上書きされます。

## Marketoを使用してアカウントを作成できますか。{#can-i-create-an-account-using-marketo}

いいえ. Marketoは、Dynamicsでアカウントを作成できません。

## どのフィールドがMarketoと同期しますか。{#which-fields-will-sync-to-marketo}

[設定中に、同期するフィールドを選択](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)できます。 ただし、Marketoは、Dynamics同期ユーザーがアクセスできるフィールドのみを同期します。

## Dynamicsの[アカウント]フィールドを変更すると、各連絡先の[データ値の変更]アクティビティログが生成されますか。 {#does-a-change-in-an-account-field-in-dynamics-results-in-a-change-data-value-activity-log-for-each-contact}

ほとんどはそうです。 ただし、アカウントに5,000個を超える連絡先があり、そのアカウントのフィールドがDynamicsで変更された場合は、変更を同期しますが、5,000個を超える連絡先のアクティビティは記録されません。
