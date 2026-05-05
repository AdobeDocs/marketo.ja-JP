---
unique-page-id: 2360253
description: 管理者メールの「Web ページとして表示」リンクテキストとHTMLをカスタマイズして、必要な変数を維持します。
title: 「Web ページとして表示」メッセージの編集
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: df76402e5fb0c002afeb04d41c52801be67a7136
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 52%

---

# 「Web ページとして表示」メッセージの編集 {#edit-the-view-as-web-page-message}

「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」テキストを編集する方法について説明します。

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
   >以下の変数は重要です。 削除しないでください。
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >2つ目の部分`##MKT_TOK##`は、そのユーザーの[!UICONTROL Munchkin] Cookieです。 これにより、オーディエンスがリンクをクリックしたときに適切に追跡されます。

1. 「**[!UICONTROL Web ページとして表示（HTML）]**」と「**[!UICONTROL Web ページとして表示（テキスト）]**」バージョンを適切に編集し、「**[!UICONTROL 変更を保存]**」をクリックします。

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>以下は避けるようにします。
>
>* いずれかの HTML ボックスに付加的な URL を追加する
>* テキストバージョンに HTML コードを配置する

テストメールを送信して、フォーマットを確認します。

## デフォルトの「Web ページとして表示」テキスト {#default-view-as-web-page-text}

デフォルトのシステム「[!UICONTROL Web ページとして表示]」に戻す必要がある場合は、次の手順をコピーまたはペーストします。

**[!UICONTROL Web ページとして表示（HTML）]**：

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL Web ページとして表示（テキスト）]**：

この電子メールをWeb ページとして表示するには、次のアドレスに移動します。
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
