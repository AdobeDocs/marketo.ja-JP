---
description: 動的フィールドでテンプレートが入力されない場合のトラブルシューティング。 結合フィールドのSalesforce接続とフィールドマッピングを確認します。
title: 動的フィールドに入力されないのはなぜですか？
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
TQID: https://experienceleague.adobe.com/UNfP0KLmX5JMdFTfSS1fuEssjNFLoXeq41wVFJzvcbE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 312
ht-degree: 73%

---

# 動的フィールドに入力されないのはなぜですか？ {#why-arent-my-dynamic-fields-filling-out}

動的フィールドは、テンプレートを使用している場合にのみ機能します。 1 回限りのメールでは、これらは記入されません。

## 確認内容 {#what-to-check}

セールスインサイトアクションには、基本、カスタム、Salesforce の 3 つのタイプの動的フィールドがあります。 基本とカスタムの両方が [web アプリケーション](https://toutapp.com/login){target="_blank"}から取り込む情報を探します。 Web アプリケーションに情報が存在しない場合、フィールドは空白になります。 Salesforce フィールドは、[Salesforce.com](https://salesforce.com){target="_blank"} から情報を取り込みます。

**[!DNL Salesforce] フィールドのトラブルシューティング**

[!DNL Salesforce] フィールド：例：`{{sfdc_account_name}}`

* Sales Insight Actionsで適切にフックアップされていることを確認します。 [設定] （<https://toutapp.com/login{target="_blank"}> ページに移動し、CRMの横にある&#x200B;**管理**&#x200B;をクリックします。

**基本フィールドとカスタムフィールドのトラブルシューティング**

Marketo セールスインサイト Actions 基本フィールド：例えば、`{{company}}`

Marketo セールスインサイト Actions カスタムフィールド：例えば、`{{custom_field_favorite_movie}}`

* 動的フィールドを参照するには、取引先責任者の[人物ページ](https://toutapp.com/next#relationships){target="_blank"}にある対応するフィールドを保存する必要があります。 例えば、Maryにメールを送信し、`{{company}}` フィールドを使用しているが、彼女の連絡先レコードが会社をリストしていない場合、それを入力することはできません。

## すべての動的フィールドに値が入力されずにメールが送信された理由 {#why-did-my-email-send-without-populating-all-dynamic-fields}

メールの動的フィールドをすべて入力できない場合、[!DNL Sales Insight Actions] はメールの送信を停止します。 **ただし**、このルールにはいくつかの例外があります。 一部のフィールドは空白で送信されるか、値が見つかった場合は値を自動入力します。 これらのフィールドと、フィールドに値を入力できない場合の反応を以下に示します。

`{{first_name}}` = 空白

`{{last_name}}` =空白

`{{title}}` = 空白

`{{company}}` =「会社」

`{{friendly_company}}` =「会社」

>[!NOTE]
>
>「`{{first_name}}`」フィールドは、[!DNL Sales Insight Actions] と [!DNL Salesforce] の両方を検索して情報の取り込みを試みます。 このリストの他のフィールドはすべて、[!DNL Sales Insight Actions] のみ検索してフィールドに入力されます。
