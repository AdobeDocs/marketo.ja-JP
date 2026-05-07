---
unique-page-id: 14352602
description: Sales Connectで動的フィールドが入力されない場合にヘルプを表示します。 結合フィールドに空白または誤ったデータが表示される理由をトラブルシューティングします。
title: 動的フィールドが入力されない場合の対処
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 76%

---

# 動的フィールドが入力されない場合の対処 {#my-dynamic-fields-arent-filling-out}

動的フィールドは、テンプレートを使用している場合にのみ機能します。 1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

[!DNL Sales Connect] には、基本、カスタム、[!DNL Salesforce] の 3 つのタイプの動的フィールドがあります。 基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login)から取り込む情報を探します。 Web アプリケーションに情報が存在しない場合、フィールドは空白になります。 [!DNL Salesforce] フィールドは、[Salesforce.com](https://salesforce.com) から情報を取り込みます。

**[!DNL Salesforce] フィールドのトラブルシューティング**

[!DNL Salesforce] フィールド：例：`{{sfdc_account_name}}`

* [!DNL Sales Connect]が正しく接続されていることを確認してください。 [設定](https://toutapp.com/login)ページに移動し、CRM の横にある「**[!UICONTROL 管理]**」をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Tout 基本フィールド：例 `{{company}}`

Tout カスタムフィールド：例 `{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、取引先責任者の[人物ページ](https://toutapp.com/next#relationships)にある対応するフィールドを保存する必要があります。 例えば、Maryにメールを送信し、`{{company}}` フィールドを使用しているが、彼女の連絡先レコードが会社をリストしていない場合、それを入力することはできません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メールの動的フィールドをすべて入力できない場合、[!DNL Sales Connect] はメールの送信を停止します。 **ただし**、このルールにはいくつかの例外があります。 一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。 これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>「`{{first_name}}`」フィールドは、[!DNL Sales Connect] と [!DNL Salesforce] の両方を検索して情報の取り込みを試みます。 このリストの他のフィールドはすべて、[!DNL Sales Connect] のみ検索してフィールドに入力されます。
