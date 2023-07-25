---
unique-page-id: 2360253
description: 「Web ページとして表示」メッセージの編集 - Marketo ドキュメント - 製品ドキュメント
title: 「Web ページとして表示」メッセージの編集
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 90%

---

# 「Web ページとして表示」メッセージの編集 {#edit-the-view-as-web-page-message}

「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」テキストを編集する必要がある場合は、次の手順に従います。

>[!NOTE]
>
>**管理者権限が必要**

## 「Web ページとして表示」メッセージの編集 {#edit-the-view-as-web-page-message-1}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. 「**[!UICONTROL メール]**」をクリックします。

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >次の変数は重要です。削除しないでください。
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >2 つ目の部分 `##MKT_TOK##` は、その人物の munchkin cookie です。リンクをクリックすると、適切に cookie が使用されるようにするものです。

1. 「**[!UICONTROL Web ページとして表示（HTML）]**」と「**[!UICONTROL Web ページとして表示（テキスト）]**」バージョンを適切に編集し、「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>以下は避けるようにします。
>
>* いずれかの HTML ボックスに付加的な URL を追加する
>* テキストバージョンに HTML コードを配置する

これで手順は完了です。フォーマットを確認するためにテストメールを送信します。

## デフォルトの「Web ページとして表示」テキスト {#default-view-as-web-page-text}

デフォルトのシステム「 」に戻す必要がある場合[!UICONTROL ウェブページとして表示]「」で、次をコピー&amp;ペーストします。

**[!UICONTROL ウェブ ページ (HTML) として表示]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL ウェブ ページ (テキスト) として表示]**:

このメールをウェブページとして閲覧するには、次のアドレスに移動してください:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

これで完了です。
