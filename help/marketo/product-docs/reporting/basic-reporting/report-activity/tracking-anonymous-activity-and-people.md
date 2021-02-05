---
unique-page-id: 2360181
description: 匿名アクティビティと人物の追跡 — Marketto Docs — 製品ドキュメント
title: 匿名アクティビティと人物の追跡
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# 匿名アクティビティと人物の追跡{#tracking-anonymous-activity-and-people}

誰かが初めてMarketorの[ランディングページ](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（またはWebサイト上の[マンチキン追跡コード](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つページ）を訪問したとき、Marketorは&#x200B;*匿名* *アクティビティ*&#x200B;を作成し、ブラウザーcookieを使用して追跡します。 訪問者が識別されると、その訪問者が個人となり、ブラウザーのcookieに関連付けられた履歴が結合されます。

1. 匿名アクティビティは、誰かが

   * 初めてマーケットランディングページ[に訪問します。](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)
   * [マンチキン追跡](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つサイトのページを訪問します。
   * Marketor電子メールの[表示をWebページ](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)リンクとしてクリックします。

   >[!NOTE]
   >
   >Marketo Eメール内の他のリンクとは異なり、Webページとしての表示は電子メールクリックとして追跡されません。

   匿名アクティビティは、次のような場合に、新しい人または既存の人に結合されます。

   * マーケティング担当者の電子メール](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)内の[リンクをクリックします。
   * Marketor [フォーム](http://docs.marketo.com/display/docs/forms)に入力します。
   * 匿名アクティビティを既知のレコードに関連付けるには、Marketoの[REST API](http://developers.marketo.com/rest-api/lead-database/leads/)または[Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API（開発者用）を使用します。

   データベース内の1つの名前が多数のcookieに結び付けられる可能性があるのは、訪問者がサイトの訪問に多くの場合、異なるデバイスやブラウザーを使用するからです。

   >[!NOTE]
   >
   >匿名レコードが新しいまたは既存の人物レコードに結合されると、カスタムフィールドの値は&#x200B;**引き継がれません。**

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Webレポートでの人または匿名訪問者の表示](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**ディープダイブ**
   >
   >
   >[基本レポート](http://docs.marketo.com/display/docs/basic+reporting)の詳細を表示します。

