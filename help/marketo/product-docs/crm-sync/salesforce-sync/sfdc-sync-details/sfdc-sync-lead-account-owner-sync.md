---
unique-page-id: 2953463
description: SFDC 同期 - リード／アカウント所有者の同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - リード／アカウント所有者の同期
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '213'
ht-degree: 100%

---

# SFDC 同期：リード／アカウントの所有者の同期 {#sfdc-sync-lead-account-owner-sync}

リード／アカウント所有者の同期は、技術的には Salesforce の「ユーザー」テーブルを同期することですが、これを「リード／アカウント所有者」フィールドと呼ぶことにします。

## Marketo と同期するのはどのフィールドですか？ {#which-fields-will-sync-to-marketo}

Marketo に同期された各ユーザーに対して、次の所有者フィールドも同期します。

* セールス所有者の名
* セールス所有者の姓
* セールス所有者の敬称
* セールス所有者の電話番号
* セールス所有者のメールアドレス

各連絡先に対して、上記の 5 つのリード所有者フィールドと、次のアカウント所有者フィールドを同期します。

* アカウント所有者の名
* アカウント所有者の姓
* アカウント所有者のメールアドレス

## Marketo でリード所有者を変更できますか？ {#can-i-change-the-lead-owner-in-marketo}

もちろんです。[所有者を変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)フローアクションを使用するだけです。

>[!NOTE]
>
>[リードの詳細ページを使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)を使用して所有者情報を変更することはできません。

## このデータを使用して何ができますか？ {#what-can-i-do-with-this-data}

このデータを使用する理由は、次のようにたくさんあります。

* セールス所有者による、署名入りのパーソナライズされたメール送信
* 特定のセールス担当者に対するマーケティングのフィルタリングや効果の分析
* Marketo の割り当て（および再割り当て）ルール
* [所有者を変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)、[リードを SFDC に同期](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)、[タスクを作成](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)の各フローアクションで使用

Marketo は、Salesforce との同期において業界でも極めて優れています。
