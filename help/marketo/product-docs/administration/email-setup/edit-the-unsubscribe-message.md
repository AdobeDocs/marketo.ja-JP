---
unique-page-id: 2360251
description: 配信停止メッセージの編集 — Marketoドキュメント — 製品ドキュメント
title: 登録解除メッセージの編集
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: 931b42d7266b9c57308567527042dfcad9847993
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 17%

---

# 登録解除メッセージの編集 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**管理者権限が必要**

マーケティングメールを送信する際 ([操作](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md))、配信停止テキストおよびリンクが下部に追加されます。 デフォルト値は変更できます。 手順は以下のとおりです。

## 登録解除メッセージの編集 {#edit-the-unsubscribe-message-1}

1. の下 **管理者**&#x200B;をクリックし、 **電子メール**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >次の変数は重要です。 削除しないでください。
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. を編集します。 **配信停止HTML** および **配信停止テキスト** バージョンを選択し、「 」をクリックします。 **変更を保存**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   あった。 _必ずテストを実施してください。_ マーケティングメールによる配信停止リンクの破損を防ぎます。

>[!TIP]
>
>E メール内の配信停止HTMLの位置は、 [トークン](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## デフォルトの配信停止テキスト {#default-unsubscribe-text}

デフォルトのシステム配信停止に戻す必要がある場合は、次をコピー&amp;ペーストします。

配信停止HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` 配信停止テキスト：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[「web ページとして表示」メッセージの編集](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
