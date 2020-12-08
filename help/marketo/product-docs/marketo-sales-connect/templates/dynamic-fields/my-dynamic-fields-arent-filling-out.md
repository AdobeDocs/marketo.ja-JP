---
unique-page-id: 14352602
description: 動的フィールドに入力できない — Marketo Docs — 製品ドキュメント
title: 動的フィールドに入力できない
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# 動的フィールドに入力できない {#my-dynamic-fields-arent-filling-out}

動的フィールドは、テンプレートを使用している場合にのみ機能します。 1回限りの電子メールでは、それらは記入されません。

## 確認内容 {#what-to-check}

Sales Connectには、次の3種類の動的フィールドがあります。基本、カスタム、Salesforce。 「基本」と「カスタム」はどちらも、 [Webアプリケーションから情報を取り込むように見えます](http://toutapp.com/login)。 Webアプリケーションに情報が存在しない場合、フィールドは空白になります。 Salesforceフィールドは、 [Salesforce.comから情報を取り込みます](http://salesforce.com)。

`**Troubleshooting Salesforce Fields**`

Salesforceフィールド：例えば `{{sfdc_account_name}}`

* Sales Connectとの接続が正しく行われていることを確認します。 「 [設定](http://toutapp.com/next#settings) 」ページに移動し、CRMの横にある「 **管理** 」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout Basic Fields:例えば `{{company}}`

カスタムフィールドを出力：例えば `{{custom_field_favorite_movie}}`

* 動的フィールド `he corresponding field needs to be saved for your contact` を参照するための、 [](http://toutapp.com/next#relationships) 人ページ内のT。 例えば、Maryに電子メールを送信し、この `{{company}}` フィールドを使用している場合、連絡先レコードが会社をリストしていないと、その情報を入力できません。

## すべての動的フィールドに値が入力されないで電子メールが送信されたのはなぜですか。 {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connectは、電子メールにすべての動的フィールドを入力できない場合、電子メールの送信を停止します。 **ただし**、このルールにはいくつかの例外があります。 一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。 以下に、これらのフィールドと、そのフィールドに値を入力できない場合の反応を示します。

`{{first_name}}` =空白

`{{last_name}}` =空白

`{{title}}` =空白

`{{company}}` = &quot;会社&quot;

`{{friendly_company}}` = &quot;会社&quot;

>[!NOTE]
>
>この `{{first_name}}` フィールドは、Sales ConnectとSalesforceの両方を参照して情報を取り込もうとします。 このリストの他のすべてのフィールドは、Sales Connectを参照してフィールドに入力するだけです。

