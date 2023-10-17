---
unique-page-id: 1146958
description: アラートの送信 - Marketo ドキュメント - 製品ドキュメント
title: アラートの送信
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 75%

---

# アラートの送信 {#send-alert}

## 概要 {#overview}

Marketo は、人物情報を記載したメールアラート（セールス所有者、パートナー、またはその他の人）を誰にでも送信できます。「[!UICONTROL アラートの送信]&quot;フローステップ。

![](assets/one-1.png)

## 使用方法 {#usage}

1. 送信するメールを探して選択します。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >メールアラートには、すべてのヘッダー情報が含まれ、「**[!UICONTROL 承認済み]**」ステートである必要があります。

1. 「プレビュー」アイコンをクリックして、正しいメールを選択していることを確認できます。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >必ず[!UICONTROL アラート情報の送信]」トークンがメールに含まれています。

1. アラート受信者を選択します。次の項目を選択できます。 [!UICONTROL セールス所有者] または [!UICONTROL アカウント所有者].

   ![](assets/four-2.png)

1. 必要に応じて、他のメールアドレスを追加します（コンマまたはセミコロンで区切ります）。

   ![](assets/five.png)

   >[!TIP]
   >
   >トリガーキャンペーンでは、値が有効なメールアドレスである限り、`{{lead.Territory Owner}}` や `{{my.Alert Recipient}}` といった「**[!UICONTROL 他のメールへ]**」トークンを使用できます。のトークン **[!UICONTROL 他のメールへ]** はバッチキャンペーンでは機能しません。

>[!MORELIKETHIS]
>
>[メールの作成](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
