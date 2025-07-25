---
description: 動的フィールドに入力されないのはなぜですか？- Marketo ドキュメント - 製品ドキュメント
title: 動的フィールドに入力されないのはなぜですか？
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 83%

---

# 動的フィールドに入力されないのはなぜですか？ {#why-arent-my-dynamic-fields-filling-out}

動的フィールドは、テンプレートを使用する場合にのみ機能します。1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

Sales Insight Actions には、基本、カスタム、Salesforce の 3 つのタイプの動的フィールドがあります。基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login){target="_blank"}から取り込む情報を探します。Web アプリケーションに情報が存在しない場合、フィールドは空白になります。Salesforce フィールドは、[Salesforce.com](https://salesforce.com){target="_blank"} から情報を取り込みます。

**[!DNL Salesforce] フィールドのトラブルシューティング**

[!DNL Salesforce] フィールド：例：`{{sfdc_account_name}}`

* このフィールドが Sales Insight Actions と正しく接続されていることを確認します。[設定]&#x200B;(https://toutapp.com/login{target="_blank"}ページに移動し、CRM の横にある「**管理**」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Marketo Sales Insight Actions 基本フィールド：例えば、`{{company}}`

Marketo Sales Insight Actions カスタムフィールド：例えば、`{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、取引先責任者の[人物ページ](https://toutapp.com/next#relationships){target="_blank"}にある対応するフィールドを保存する必要があります。例えば、Mary にメールを送信し、`{{company}}` フィールドを使用しているが、その取引先責任者レコードに会社がリストされていない場合、フィールドには入力されません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メ [!DNL Sales Insight Actions] ル内のすべての動的フィールドに値を入力できない場合、メールの送信が停止されます。 **ただし**、このルールにはいくつかの例外があります。一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>`{{first_name}}` フィールドは、情報を取り込もうとして [!DNL Sales Insight Actions] と [!DNL Salesforce] の両方を検索します。 このリスト内の他のすべてのフィールドは、フィールドに値を入力するた [!DNL Sales Insight Actions] にのみ参照されます。
