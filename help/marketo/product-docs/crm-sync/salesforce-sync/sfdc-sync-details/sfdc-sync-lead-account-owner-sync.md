---
unique-page-id: 2953463
description: SFDC同期 — リード/アカウント所有者の同期 —Marketoドキュメント — 製品ドキュメント
title: SFDC同期 — リード/アカウント所有者の同期
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# SFDC同期：リード/アカウント所有者の同期{#sfdc-sync-lead-account-owner-sync}

これらは技術的にはSalesforceの「ユーザー」テーブルを同期していますが、リード/アカウント所有者フィールドと呼ばれます。

## どのフィールドがMarketoと同期しますか。{#which-fields-will-sync-to-marketo}

Marketoに同期した各ユーザーに対して、次の所有者フィールドも同期します。

* セールス所有者の名
* セールス所有者の姓
* 販売所有者の役職
* セールス所有者の電話番号
* セールス所有者のメールアドレス

連絡先ごとに、上記5つのリード所有者フィールドと次のアカウント所有者フィールドを同期します。

* アカウント所有者の名
* アカウント所有者の姓
* アカウント所有者のメールアドレス

## Marketoのリードオーナーを変更できますか。{#can-i-change-the-lead-owner-in-marketo}

絶対に、[所有者の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)フローアクションを使用してください。

>[!NOTE]
>
>[個人の詳細ページ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)を使用して所有者情報を変更することはできません。

## このデータを使用して何ができますか。{#what-can-i-do-with-this-data}

このデータを使用する理由は、次のとおりです。

* 販売所有者からの署名付きのパーソナライズされた電子メールの送信
* マーケティングや効果の分析を行うために、特定の営業担当者に対してフィルタを適用
* Marketoの割り当て（および再割り当て）ルール
* [所有者の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)、[個人をSFDCに同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)、[タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)の各フローアクションで使用します。

Marketoは、Salesforceとの同期を素晴らしくしている。 他の誰も上手くやれない！
