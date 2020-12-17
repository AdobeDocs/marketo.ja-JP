---
unique-page-id: 2360251
description: 購読解除メッセージの編集 — Marketto Docs — 製品ドキュメント
title: 登録解除メッセージの編集
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# 登録解除メッセージの編集{#edit-the-unsubscribe-message}

>[!NOTE]
>
>**必要な管理者権限**

マーケティング電子メール（[操作](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)以外）を送信すると、登録解除のテキストとリンクが下部に追加されます。 デフォルト値は変更できます。 これが方法です。

## 登録解除メッセージの編集{#edit-the-unsubscribe-message-1}

1. 「**管理者**」で、「**電子メール**」をクリックします。

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >次の変数が重要です。 削除しないでください。
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscribe=1&amp;mkt_tok=#MKT_TOK##**


1. 「**HTMLの登録解除**」および「**購読解除テキスト**」のバージョンを編集し、「**変更を保存**」をクリックします。

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   あっある。 **必ずテストして！** マーケティング電子メールが購読解除リンクを破壊しないようにする。

>[!TIP]
>
>[tokens](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)を使用して、電子メール内の登録解除HTMLの位置をカスタマイズできます。

## デフォルトの登録解除テキスト{#default-unsubscribe-text}

デフォルトのシステム登録解除に戻す必要がある場合は、次をコピー&amp;ペーストします。

HTMLの登録解除：
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>`登録解除テキスト：
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>* [「表示をWebページとして」メッセージの編集](edit-the-view-as-web-page-message.md)

>



