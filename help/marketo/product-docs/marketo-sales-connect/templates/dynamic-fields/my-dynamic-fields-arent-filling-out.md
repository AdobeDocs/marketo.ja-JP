---
unique-page-id: 14352602
description: 動的フィールドが入力されない場合の対処 - Marketo ドキュメント - 製品ドキュメント
title: 動的フィールドが入力されない場合の対処
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 74%

---

# 動的フィールドが入力されない場合の対処 {#my-dynamic-fields-arent-filling-out}

動的フィールドは、テンプレートを使用する場合にのみ機能します。1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

[!DNL Sales Connect] には、基本、カスタム、[!DNL Salesforce] の 3 種類の動的フィールドがあります。 基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login)から取り込む情報を探します。Web アプリケーションに情報が存在しない場合、フィールドは空白になります。[!DNL Salesforce] フィールドは [Salesforce.com](https://salesforce.com) から情報を取り込みます。

**[!DNL Salesforce] フィールドのトラブルシューティング**

[!DNL Salesforce] フィールド：例：`{{sfdc_account_name}}`

* [!DNL Sales Connect] でちゃんとフックされていることを確認してください。 [設定](https://toutapp.com/login)ページに移動し、CRM の横にある「**[!UICONTROL 管理]**」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout 基本フィールド：例 `{{company}}`

Tout カスタムフィールド：例 `{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、取引先責任者の[人物ページ](https://toutapp.com/next#relationships)にある対応するフィールドを保存する必要があります。例えば、Mary にメールを送信し、`{{company}}` フィールドを使用しているが、その取引先責任者レコードに会社がリストされていない場合、フィールドには入力されません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メ [!DNL Sales Connect] ル内のすべての動的フィールドに値を入力できない場合、メールの送信が停止されます。 **ただし**、このルールにはいくつかの例外があります。一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>`{{first_name}}` フィールドは、情報を取り込もうとして [!DNL Sales Connect] と [!DNL Salesforce] の両方を検索します。 このリスト内の他のすべてのフィールドは、フィールドに値を入力するた [!DNL Sales Connect] にのみ参照されます。
