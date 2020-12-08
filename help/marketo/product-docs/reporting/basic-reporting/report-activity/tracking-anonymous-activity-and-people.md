---
unique-page-id: 2360181
description: 匿名アクティビティと人物の追跡 — Marketto Docs — 製品ドキュメント
title: 匿名アクティビティと人物の追跡
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# 匿名アクティビティと人物の追跡 {#tracking-anonymous-activity-and-people}

Marketo [ランディングページ](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (または、Munchkin追跡コードを含むWebサイト上のページ [)を初めて訪問すると、Marketoは](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)匿名 *アクティビティを作成し、訪問者がブラウザのcookieを使用して追跡するように*** します。 訪問者が識別されると、その訪問者が個人となり、ブラウザーのcookieに関連付けられた履歴が結合されます。

1. 匿名アクティビティは、誰かが

   * マーケティング [ランディングページ](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) 、初めて訪問します。
   * マンチキン追跡を含むサイトのページ [を訪問します](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。
   * マーケティング担当者の電子メール内で、 [表示を「Webページ](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 」リンクとしてクリックします。

   >[!NOTE]
   >
   >Marketo Eメール内の他のリンクとは異なり、Webページとしての表示は電子メールクリックとして追跡されません。

   匿名アクティビティは、次のような場合に、新しい人または既存の人に結合されます。

   * マーケティング担当者の電子メール内の [リンクをクリックします](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)。
   * マーケティング担当者の [フォームに入力します](http://docs.marketo.com/display/docs/forms)。
   * Marketoの [REST API](http://developers.marketo.com/rest-api/lead-database/leads/)[（開発者向け）または](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) Munchkin API（開発者向け）を使用して、匿名アクティビティを既知のレコードに関連付けます。

   データベース内の1つの名前が多数のcookieに結び付けられる可能性があるのは、訪問者がサイトの訪問に多くの場合、異なるデバイスやブラウザーを使用するからです。

   >[!NOTE]
   >
   >匿名レコードが新しい人レコードまたは既存の人物レコードに結合されると、カスタムフィールドの値は **転送されません** 。

   >[!NOTE]
   >
   >**関連記事**
   >
   >    
   >    
   >    * [Webレポートでの人または匿名訪問者の表示](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**ディープダイブ**
   >
   >
   >[基本レポートの詳細を表示します](http://docs.marketo.com/display/docs/basic+reporting)。

