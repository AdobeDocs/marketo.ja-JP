---
unique-page-id: 2953463
description: SFDC 同期 - リード／アカウント所有者の同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード／アカウント所有者の同期
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 84%

---

# SFDC 同期：リード／アカウントの所有者の同期 {#sfdc-sync-lead-account-owner-sync}

これらは技術的には [!DNL Salesforce] の「ユーザー」テーブルを同期していますが、リード/アカウント所有者フィールドと呼ぶことにします。

## Marketo Engageに同期されるフィールドはどれですか？ {#which-fields-will-sync-to-marketo-engage}

Marketo に同期された各ユーザに対して、次の所有者フィールドも同期します。

* セールス所有者の名
* セールス所有者の姓
* セールス所有者の職位
* セールス所有者の電話番号
* セールス所有者のメールアドレス

各取引先責任者に対して、上記の 5 つのリード所有者フィールドと、次のアカウント所有者フィールドを同期します。

* アカウント所有者の名
* アカウント所有者の姓
* アカウント所有者のメールアドレス

## Marketo でリード所有者を変更できますか？ {#can-i-change-the-lead-owner-in-marketo}

もちろんです。[所有者を変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}フローアクションを使用するだけです。

>[!NOTE]
>
>[リードの詳細ページを使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}を使用して所有者情報を変更することはできません。

## このデータを使用して何ができますか？ {#what-can-i-do-with-this-data}

このデータを使用する理由は、次のようにたくさんあります。

* セールス所有者による、署名入りのパーソナライズされたメール送信
* 特定のセールス担当者に対するマーケティングのフィルタリングや効果の分析
* Marketo の割り当て（および再割り当て）ルール
* [所有者を変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}、[リードを SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}、[タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}の各フローアクションで使用

Marketoは素晴らしい [!DNL Salesforce] 同期を持っています。 業界でも極めて優れています。
