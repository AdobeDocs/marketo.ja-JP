---
unique-page-id: 1146958
description: アラートの送信 — Marketto Docs — 製品ドキュメント
title: アラートの送信
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# アラートの送信 {#send-alert}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

## 概要 {#overview}

Marketorは、販売所有者、パートナー、その他の人に、個人情報を含む電子メールアラートを送信できます。 [ **アラートの** 送信]フローステップを使用します。

![](assets/one-1.png)

## 使用状況 {#usage}

1. 送信する電子メールを探して選択します。

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >電子メールアラートには、すべてのヘッダー情報が含まれ、「 **承認済み** 」状態になっている必要があります。

1. プレビューアイコンをクリックして、正しい電子メールが選択されていることを確認できます。

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >電子メールの「 **アラート情報の送信** 」トークンを必ず使用してください。

1. アラート受信者を選択します。 「販売所有者」または「アカウント所有者」を選択できます。

   ![](assets/four-2.png)

1. 必要に応じて、必要に応じて、他の電子メールアドレスを追加します（コンマまたはセミコロンで区切ります）。

   ![](assets/five.png)

   >[!TIP]
   >
   >トリガーキャンペーンでは、値が有効な電子メールアドレスである限り、 **「他の電子メール** 」 `{{lead.Territory Owner}}` にあるトークン(例えば、値 `{{my.Alert Recipient}}` )を使用できます。 「 **他の電子メール** へのトークン」は、バッチキャンペーンでは機能しません。

それだ！ これで、「 **アラートの送信** 」フロー手順の使用方法がわかりました。

>[!NOTE]
>
>**関連記事**
>
>[電子メールの作成](../../../../product-docs/email-marketing/general/creating-an-email/create-an-email.md)

