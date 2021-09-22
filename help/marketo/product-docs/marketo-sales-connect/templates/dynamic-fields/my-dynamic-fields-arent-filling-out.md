---
unique-page-id: 14352602
description: 動的フィールドが入力されない場合の対処 - Marketo ドキュメント - 製品ドキュメント
title: 動的フィールドが入力されない場合の対処
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
source-git-commit: ''
workflow-type: ht
source-wordcount: '301'
ht-degree: 100%

---

# 動的フィールドが入力されない場合の対処 {#my-dynamic-fields-arent-filling-out}

動的フィールドは、テンプレートを使用する場合にのみ機能します。1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

Sales Connect には、基本、カスタム、Salesforce の 3 つのタイプの動的フィールドがあります。基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login)から取り込む情報を探します。Web アプリケーションに情報が存在しない場合、フィールドは空白になります。Salesforce フィールドは、[Salesforce.com](https://salesforce.com) から情報を取り込みます。

**Salesforce フィールドのトラブルシューティング**

Salesforce フィールド：例 `{{sfdc_account_name}}`

* このフィールドが Sales Connect と正しく接続されていることを確認します。[設定](https://toutapp.com/login)ページに移動し、CRM の横にある「**管理**」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout 基本フィールド：例 `{{company}}`

Tout カスタムフィールド：例 `{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、連絡先の[リードページ](https://toutapp.com/next#relationships)にある対応するフィールドを保存する必要があります。例えば、Mary にメールを送信し、`{{company}}` フィールドを使用しているが、その連絡先レコードに会社がリストされていない場合、フィールドには入力されません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メールの動的フィールドをすべて入力できない場合、Sales Connect はメールの送信を停止します。**ただし**、このルールにはいくつかの例外があります。一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>`{{first_name}}` フィールドは、Sales Connect と Salesforce の両方を検索して情報の取り込みを試みます。このリストの他のフィールドはすべて、Sales Connect のみ検索してフィールドに入力されます。
