---
unique-page-id: 2953459
description: SFDC同期 — アカウントの同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 — アカウントの同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# SFDC同期：アカウントの同期{#sfdc-sync-account-sync}

また、Marketorは、アカウント情報をSalesforceと同期します。 知っておくべきことがいくつかあります！

## 情報の同期方法{#which-way-does-the-information-sync}

次の1つの方法のみ：をSFDCからMarketoに送信します。

## アップデートの動作{#how-do-the-updates-work}

Marketorの担当者の「アカウント」フィールドを更新すると、Marketorのそのアカウントに属するすべての担当者の値が変更されます。 SFDCとは同期されません。 ただし、次回SFDCでアカウントが更新されたときは、Marketoのすべてのアカウント情報が変更によって上書きされます。

## 連絡先は複数のアカウントに属することができますか？ {#can-a-contact-belong-to-multiple-accounts}

いいえ。 アカウントには多数の連絡先を設定でき、連絡先には1つのアカウントしか設定できません。

## Marketoからアカウントを作成できますか。{#can-i-create-accounts-from-marketo}

ほとんどは違う。 ただし、個人に対して[個人](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)のコンバートのフロー手順を使用すると、新しい連絡先、新しいアカウント、新しいオポチュニティが作成されます。

>[!CAUTION]
>
>このフローステップの使用例は非常に限られています。 分からないなら、使わない方がよいでしょう。

## Salesforceのアカウントフィールドを変更すると、各連絡先のデータ値の変更アクティビティログが生成されますか。 {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

ほとんどはそうです。 ただし、アカウントに5,000件を超える連絡先があり、そのアカウントのフィールドがSFDCに変更された場合は、変更を同期しますが、5,000件を超える連絡先のアクティビティは記録しません。
