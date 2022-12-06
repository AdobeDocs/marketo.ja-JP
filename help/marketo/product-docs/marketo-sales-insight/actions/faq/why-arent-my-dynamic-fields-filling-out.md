---
description: 動的フィールドに入力されないのはなぜですか？ - Marketo ドキュメント - 製品ドキュメント
title: 動的フィールドに入力されないのはなぜですか？
hide: true
hidefromtoc: true
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: f77a076c243c25f3bff98a82751f51c464712795
workflow-type: ht
source-wordcount: '309'
ht-degree: 100%

---

# 動的フィールドに入力されないのはなぜですか？ {#why-arent-my-dynamic-fields-filling-out}

動的フィールドは、テンプレートを使用する場合にのみ機能します。1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

Sales Insight Actions には、基本、カスタム、Salesforce の 3 つのタイプの動的フィールドがあります。基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login)から取り込む情報を探します。Web アプリケーションに情報が存在しない場合、フィールドは空白になります。Salesforce フィールドは、[Salesforce.com](https://salesforce.com) から情報を取り込みます。

**Salesforce フィールドのトラブルシューティング**

Salesforce フィールド：例 `{{sfdc_account_name}}`

* このフィールドが Sales Insight Actions と正しく接続されていることを確認します。[設定](https://toutapp.com/login)ページに移動し、CRM の横にある「**管理**」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout 基本フィールド：例 `{{company}}`

Tout カスタムフィールド：例 `{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、取引先責任者の[人物ページ](https://toutapp.com/next#relationships)にある対応するフィールドを保存する必要があります。例えば、Mary にメールを送信し、`{{company}}` フィールドを使用しているが、その取引先責任者レコードに会社がリストされていない場合、フィールドには入力されません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メールの動的フィールドをすべて入力できない場合、Sales Insight Actions メールの送信を停止します。**ただし**、このルールにはいくつかの例外があります。一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>`{{first_name}}` フィールドは、Sales Insight Actions と Salesforce の両方を検索して情報の取り込みを試みます。このリストの他のフィールドはすべて、Sales Insight Actions のみ検索してフィールドに入力されます。
