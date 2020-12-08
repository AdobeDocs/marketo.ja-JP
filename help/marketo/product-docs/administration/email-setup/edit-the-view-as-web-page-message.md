---
unique-page-id: 2360253
description: 「Webページとしての表示」メッセージの編集 — Marketto Docs — 製品ドキュメント
title: 「表示をWebページとして」メッセージの編集
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# 「表示をWebページとして」メッセージの編集 {#edit-the-view-as-web-page-message}

「 [表示をWebページとして編集する](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」のテキストを編集する場合は、次のようにします。

>[!NOTE]
>
>**必要な管理者権限**

## 「表示をWebページとして」メッセージの編集 {#edit-the-view-as-web-page-message-1}

1. 「 **管理者**」で、「 **電子メール**」をクリックします。

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >次の変数が重要です。 削除しないでください。
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=#MKT_TOK##
   >    
   >    
   >第2部##MKT_TOK##は、その人のマンチキンcookieです。 リンクをクリックしたときに、適切にcookieを使用できることを確認します。

1. 必要に応じて、 **表示をWebページHTML** 、**表示をWebページテキスト**として編集し、「変更の **保存**」をクリックします。

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>以下は必ず避けてください。
>
>* いずれかのHTMLボックスへのURLの追加
>* テキストバージョンへのHTMLの配置

>



あっある。 フォーマットを確認するためにテスト用電子メールを送信します。

## デフォルトの「Webページとしての表示」テキスト {#default-view-as-web-page-text}

デフォルトのシステム「Webページとしての表示」に戻す必要がある場合は、次をコピー&amp;ペーストします。

**WebページHTMLとしての表示:**`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **Webページテキストとしての表示:**

この電子メールをWebページとして表示するには、次のアドレスに移動します。`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` ブーム！ 終わった。
