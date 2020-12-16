---
unique-page-id: 1147322
description: 匿名アクティビティと人について — Marketto Docs — 製品ドキュメント
title: 匿名アクティビティと人について
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 匿名アクティビティと人について {#understanding-anonymous-activity-and-people}

誰かがMarketto [L `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (またはMunchkin Tracking Codeを持つWebサイト上のページ [)を初めて訪問したとき、Marketoは*匿名*](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)** アクティビティを作成し、ブラウザーcookieを使用して追跡します。 識別されると、その訪問者が個人になり、ブラウザーのCookieに関連付けられた履歴が統合されます。

**匿名** アクティビティは、誰かが

* マーケティングランディングページに初めて訪問します。

* マンチキン追跡を含むサイトのページ [を訪問します](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)。

* マーケティング担当者の電子メール内で、 [表示を「Webページ](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 」リンクとしてクリックします。

>[!NOTE]
>
>Marketo Eメール内の他のリンクとは異なり、Webページとしての [表示は](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) 、電子メールクリックとして追跡されません。

匿名アクティビティは、次のような場合に、新しい人または既存の人に結合されます。

* マーケティング担当者の電子メール内の [リンクをクリックします](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)。
* マーケティング担当者の [フォームに入力します](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)。
* Marketoの [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) APIまたは [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（開発者向け）を使用して、匿名の人を既知のレコードに関連付けます。

データベース内の1つの名前が多数のcookieに結び付けられる可能性があるのは、訪問者がサイトの訪問に多くの場合、異なるデバイスやブラウザーを使用するからです。

>[!NOTE]
>
>匿名レコードが新しい人レコードまたは既存の人物レコードに結合されると、カスタムフィールドの値は **転送されません** 。

