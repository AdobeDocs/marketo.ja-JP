---
unique-page-id: 2953463
description: SFDC同期 — リード/アカウント所有者の同期 — Marketto Docs — 製品ドキュメント
title: SFDC同期 — リード/アカウント所有者の同期
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# SFDC同期：リード/アカウント所有者の同期{#sfdc-sync-lead-account-owner-sync}

これらは技術的にはSalesforceの「ユーザー」テーブルを同期していますが、リード/アカウント所有者フィールドと呼ばれます。

## Marketoと同期するフィールドはどれか。{#which-fields-will-sync-to-marketo}

Marketorと同期する各ユーザーに対して、次の所有者フィールドも同期します。

* 販売所有者の名
* 販売所有者の姓
* 販売所有者の役職
* 販売所有者の電話番号
* 販売所有者の電子メールアドレス

連絡先ごとに、上記5つのリード所有者フィールドと次のアカウント所有者フィールドを同期します。

* アカウント所有者の名
* アカウント所有者の姓
* アカウント所有者の電子メールアドレス

## Marketorのリード所有者を変更できますか。{#can-i-change-the-lead-owner-in-marketo}

絶対に、[所有者の変更](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)フローアクションを使用してください。

>[!NOTE]
>
>[個人の詳細ページ](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)を使用して所有者情報を変更することはできません。

## このデータを使用して何ができますか。{#what-can-i-do-with-this-data}

このデータを使用する理由は、次のとおりです。

* 販売所有者からの署名付きのパーソナライズされた電子メールの送信
* マーケティングや効果の分析を行うために、特定の営業担当者に対してフィルタを適用
* マーケティング担当者の割り当て（および再割り当て）ルール
* [所有者の変更](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)、[個人をSFDCに同期](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)、[タスクを作成](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)の各フローアクションで使用します。

Marketorは、Salesforceとの同期を素晴らしく行っています。 他の誰も上手くやれない！
