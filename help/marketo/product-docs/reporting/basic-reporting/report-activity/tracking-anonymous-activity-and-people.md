---
unique-page-id: 2360181
description: 匿名アクティビティと人物の追跡 —Marketoドキュメント — 製品ドキュメント
title: 匿名アクティビティと人物の追跡
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# 匿名アクティビティと人物の追跡{#tracking-anonymous-activity-and-people}

誰かが初めてMarketo[ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（または[マンチキン追跡コード](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つWebサイト上のページ）を訪問したとき、Marketoは&#x200B;_匿名アクティビティ_&#x200B;を作成し、ブラウザーcookieを使用して追跡します。 訪問者が識別されると、その訪問者が個人となり、ブラウザーのcookieに関連付けられた履歴が結合されます。

1. 匿名アクティビティは、誰かが

   * Marketo[ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)を初めて訪問します。
   * [マンチキン追跡](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つサイトのページを訪問します。
   * Marketoの電子メール内の[表示を「Webページ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」リンクとしてクリックします。

   >[!NOTE]
   >
   >Marketoの電子メール内の他のリンクとは異なり、ウェブページとしての表示は電子メールクリックとして追跡されません。

   匿名アクティビティは、次のような場合に、新しい人または既存の人に結合されます。

   * Marketoの電子メール](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)内の[リンクをクリックします。
   * Marketo[フォーム](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)を入力します。
   * Marketoの[REST API](https://developers.marketo.com/rest-api/lead-database/leads/)または[Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API （開発者用）を使用して、匿名アクティビティを既知のレコードに関連付けます。

   データベース内の1つの名前が多数のcookieに結び付けられる可能性があるのは、訪問者がサイトの訪問に多くの場合、異なるデバイスやブラウザーを使用するからです。

   >[!NOTE]
   >
   >匿名レコードが新しいまたは既存の人物レコードに結合されると、カスタムフィールドの値は&#x200B;**引き継がれません。**

   >[!MORELIKETHIS]
   >
   >[Webレポートでの人または匿名訪問者の表示](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
