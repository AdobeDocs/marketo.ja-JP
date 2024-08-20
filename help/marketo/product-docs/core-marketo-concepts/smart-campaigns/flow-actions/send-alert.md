---
unique-page-id: 1146958
description: アラートの送信 - Marketo ドキュメント - 製品ドキュメント
title: アラートの送信
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: ht
source-wordcount: '153'
ht-degree: 100%

---

# アラートの送信 {#send-alert}

Marketo Engage は、人物情報を記載したメールアラート（セールス所有者、パートナー、またはその他の人）を誰にでも送信できます。「[!UICONTROL アラートの送信]」フローステップを使用します。

![](assets/send-alert-1.png)

1. 送信するメールを探して選択します。

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >メールアラートには、すべてのヘッダー情報が含まれ、「**[!UICONTROL 承認済み]**」ステートである必要があります。

1. 「プレビュー」アイコンをクリックして、正しいメールを選択していることを確認できます。

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >必ず「[!UICONTROL アラート情報の送信]」トークンをメールに追加するようにします。

1. アラート受信者を選択します。「[!UICONTROL セールス所有者]」または「[!UICONTROL アカウント所有者]」を選択できます。

   ![](assets/send-alert-4.png)

1. 必要に応じて、他のメールアドレスを追加します（コンマまたはセミコロンで区切ります）。

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >トリガーキャンペーンでは、値が有効なメールアドレスである限り、`{{lead.Territory Owner}}` や `{{my.Alert Recipient}}` といった「**[!UICONTROL 他のメールへ]**」トークンを使用できます。「**[!UICONTROL 他のメールへ]**」のトークンはバッチキャンペーンでは機能しません。

>[!MORELIKETHIS]
>
>[メールの作成](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
