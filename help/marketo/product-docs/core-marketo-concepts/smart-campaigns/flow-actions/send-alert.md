---
unique-page-id: 1146958
description: アラートの送信 - Marketo ドキュメント - 製品ドキュメント
title: アラートの送信
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '167'
ht-degree: 100%

---

# アラートの送信 {#send-alert}

## 概要 {#overview}

Marketo は、人物情報を記載したメールアラート（セールス所有者、パートナー、またはその他の人）を誰にでも送信できます。「**アラートの送信**」フローステップを使用します。

![](assets/one-1.png)

## 使用方法 {#usage}

1. 送信するメールを探して選択します。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >メールアラートには、すべてのヘッダー情報が含まれ、「**承認済み**」ステートである必要があります。

1. 「プレビュー」アイコンをクリックして、正しいメールを選択していることを確認できます。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >必ず「**アラート情報の送信**」トークンをメールに追加するようにします。

1. アラート受信者を選択します。「セールス所有者」または「アカウント所有者」を選択できます。

   ![](assets/four-2.png)

1. 必要に応じて、他のメールアドレスを追加します（コンマまたはセミコロンで区切ります）。

   ![](assets/five.png)

   >[!TIP]
   >
   >トリガーキャンペーンでは、値が有効なメールアドレスである限り、`{{lead.Territory Owner}}` や `{{my.Alert Recipient}}` といった「**他のメールへ**」トークンを使用できます。「**他のメールへ**」のトークンはバッチキャンペーンでは機能しません。

これで完了です。「**アラートの送信**」フローステップの使用方法を理解できました。

>[!MORELIKETHIS]
>
>[メールの作成](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
