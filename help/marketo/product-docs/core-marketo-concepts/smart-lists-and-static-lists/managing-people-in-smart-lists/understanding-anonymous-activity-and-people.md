---
unique-page-id: 1147322
description: 匿名アクティビティと人について —Marketoドキュメント — 製品ドキュメント
title: 匿名アクティビティと人について
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# 匿名アクティビティとユーザーについて{#understanding-anonymous-activity-and-people}

Marketoのランディングページ（または、[マンチキントラッキングコード](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つWebサイトのページ）を初めて訪問したとき、Marketoは&#x200B;_匿名アクティビティ_&#x200B;を作成し、ブラウザーcookieを使用して追跡します。 識別されると、その訪問者が個人になり、ブラウザーのCookieに関連付けられた履歴が統合されます。

**匿名アクティビティは、次のような場合に作成され** ます。

* 初めてMarketoランディングページを訪問します。
* [マンチキン追跡](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つサイトのページを訪問します。
* Marketoの電子メール内の[表示を「Webページ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」リンクとしてクリックします。

>[!NOTE]
>
>Marketoの電子メール内の他のリンクとは異なり、[Webページ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)としての表示は、電子メールクリックとして追跡されません。

匿名アクティビティは、次のような場合に、新しい人または既存の人に結合されます。

* Marketoの電子メール](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)内の[リンクをクリックします。
* Marketo[フォーム](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)を入力します。
* Marketoの[SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md)または[Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API （開発者用）を使用して、匿名の人を既知のレコードに関連付けます。

データベース内の1つの名前が多数のcookieに結び付けられる可能性があるのは、訪問者がサイトの訪問に多くの場合、異なるデバイスやブラウザーを使用するからです。

>[!NOTE]
>
>匿名レコードが新しいまたは既存の人物レコードに結合されると、カスタムフィールドの値は&#x200B;**引き継がれません。**
