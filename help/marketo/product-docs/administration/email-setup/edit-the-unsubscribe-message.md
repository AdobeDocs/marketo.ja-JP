---
unique-page-id: 2360251
description: 登録解除メッセージの編集 - Marketo ドキュメント - 製品ドキュメント
title: 登録解除メッセージの編集
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: ht
source-wordcount: '139'
ht-degree: 100%

---

# 登録解除メッセージの編集 {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**管理者権限が必要**

マーケティングメールを送信する際（非[オペレーショナル](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)）、登録解除テキストおよびリンクが下部に追加されます。デフォルト値は変更できます。手順は以下のとおりです。

## 編集を行う場所 {#where-to-make-the-edit}

1. 「**[!UICONTROL 管理者]**」セクションに移動します。

   ![](assets/edit-the-unsubscribe-message-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >以下の変数は重要です。削除しないでください。
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. 「**[!UICONTROL 登録解除 HTML]**」および「**[!UICONTROL 登録解除テキスト]**」バージョンを選択し、「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/edit-the-unsubscribe-message-3.png)

   これで手順は完了です。_テストは忘れずに実行してください。_ マーケティングメールに破損した登録解除リンクがあるのは避けるべきです。

>[!TIP]
>
>メール内の登録解除 HTML の位置は、[トークン](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)を使用してカスタマイズできます。

## デフォルトの登録解除テキスト {#default-unsubscribe-text}

デフォルトのシステム登録解除に戻す必要がある場合は、以下をコピー＆ペーストします。

[!UICONTROL Unsubscribe HTML]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Unsubscribe Text]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[「Web ページとして表示」メッセージの編集](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
