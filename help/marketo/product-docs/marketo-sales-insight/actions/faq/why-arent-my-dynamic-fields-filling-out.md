---
description: 動的フィールドに入力されない理由 — Marketoドキュメント — 製品ドキュメント
title: 動的フィールドが入力されないのはなぜですか？
hide: true
hidefromtoc: true
source-git-commit: 8e31c2da9351d784e97d3d2bfe0d3d07dfab8961
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 66%

---

# 動的フィールドが入力されないのはなぜですか？ {#why-arent-my-dynamic-fields-filling-out}

動的フィールドは、テンプレートを使用する場合にのみ機能します。1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

Sales Insight アクションには、次の 3 種類の動的フィールドがあります。基本、カスタム、Salesforce。 基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login)から取り込む情報を探します。Web アプリケーションに情報が存在しない場合、フィールドは空白になります。Salesforce フィールドは、[Salesforce.com](https://salesforce.com) から情報を取り込みます。

**Salesforce フィールドのトラブルシューティング**

Salesforce フィールド：例 `{{sfdc_account_name}}`

* Sales Insight アクションと正しく接続されていることを確認します。 [設定](https://toutapp.com/login)ページに移動し、CRM の横にある「**管理**」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout 基本フィールド：例 `{{company}}`

Tout カスタムフィールド：例 `{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、連絡先の[リードページ](https://toutapp.com/next#relationships)にある対応するフィールドを保存する必要があります。例えば、Mary にメールを送信し、`{{company}}` フィールドを使用しているが、その連絡先レコードに会社がリストされていない場合、フィールドには入力されません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メールにすべてのダイナミックフィールドを入力できない場合、Sales Insight アクションはメールの送信を停止します。 **ただし**、このルールにはいくつかの例外があります。一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>この `{{first_name}}` フィールドは、Sales Insight Actions と Salesforce の両方で情報の取り込みを試みます。 このリスト内の他のすべてのフィールドは、Sales Insight アクションでフィールドに値を入力するためにのみ検索されます。
