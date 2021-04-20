---
unique-page-id: 14352602
description: 動的フィールドに入力できない —Marketoドキュメント — 製品ドキュメント
title: 動的フィールドに入力できない
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

# 動的フィールドが{#my-dynamic-fields-arent-filling-out}に入力されない

動的フィールドは、テンプレートを使用している場合にのみ機能します。 1回限りの電子メールでは、それらは記入されません。

## {#what-to-check}の確認内容

Sales Connectには、次の3種類の動的フィールドがあります。基本、カスタム、Salesforce。 「基本」と「カスタム」はどちらも、[Webアプリケーション](https://toutapp.com/login)から情報を取り込むように見えます。 Webアプリケーションに情報が存在しない場合、フィールドは空白になります。 Salesforceフィールドは、[Salesforce.com](https://salesforce.com)から情報を取り込みます。

**Salesforceフィールドのトラブルシューティング**

Salesforceフィールド：例えば`{{sfdc_account_name}}`

* Sales Connectとの接続が正しく行われていることを確認します。 [設定](https://toutapp.com/login)ページに移動し、CRMの横の&#x200B;**管理**&#x200B;をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout Basic Fields:例えば`{{company}}`

カスタムフィールドを出力：例えば`{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、[ユーザーページ](https://toutapp.com/next#relationships)に連絡先のために、対応するフィールドを保存する必要があります。 例えば、Maryに電子メールを送信し、`{{company}}`フィールドを使用しているが、連絡先レコードが会社をリストしていない場合、その情報を入力することはできません。

## すべての動的フィールドに値が入力されないで電子メールが送信されたのはなぜですか。{#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connectは、電子メールにすべての動的フィールドを入力できない場合、電子メールの送信を停止します。 **ただし**、このルールにはいくつかの例外があります。一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。 以下に、これらのフィールドと、そのフィールドに値を入力できない場合の反応を示します。

`{{first_name}}` =空白

`{{last_name}}` =空白

`{{title}}` =空白

`{{company}}` = &quot;会社&quot;

`{{friendly_company}}` = &quot;会社&quot;

>[!NOTE]
>
>`{{first_name}}`フィールドは、Sales ConnectとSalesforceの両方を検索して情報を取り込もうとします。 このリストの他のすべてのフィールドは、Sales Connectを参照してフィールドに入力するだけです。
