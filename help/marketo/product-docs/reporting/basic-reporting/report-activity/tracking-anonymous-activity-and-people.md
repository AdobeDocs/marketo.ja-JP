---
unique-page-id: 2360181
description: 匿名アクティビティとリードのトラッキング - Marketo ドキュメント - 製品ドキュメント
title: 匿名アクティビティとリードのトラッキング
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 100%

---

# 匿名アクティビティとリードのトラッキング {#tracking-anonymous-activity-and-people}

Marketo の[ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（または web サイト上で [Munchkin トラッキングコード](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つページ）に初めて訪問すると、Marketo は&#x200B;_匿名アクティビティ_&#x200B;を作成し、ブラウザー cookie を使用してトラックします。識別されると、その訪問者はリードとなり、ブラウザーの Cookie に関連付けられた履歴が結合されます。

1. 匿名アクティビティは、次の場合に作成されます。

   * 初めて Marketo の[ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)にアクセスしたとき。
   * [Munchkin トラッキング](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つサイトのページを訪問したとき。
   * Marketo メールの「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」リンクをクリックしたとき。

   >[!NOTE]
   >
   >Marketo メールの他のリンクとは異なり、「Web ページとして表示」は、メールクリックとしてはトラックされません。

   匿名アクティビティは、次の場合に、新規または既存のユーザに結合されます。

   * [Marketo メール内のリンク](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)をクリックしたとき。
   * Marketo の[フォーム](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md)に入力したとき。
   * [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) または [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API（開発者向け）を使用して、匿名のアクティビティを既知のレコードに関連付けたとき。

   異なるデバイスやブラウザーからサイトにアクセスされることが多いので、データベース内の 1 つの名前が多くの cookie に関連付けられる場合があります。

   >[!NOTE]
   >
   >匿名レコードが新しいリードレコードまたは既存のリードレコードに結合されると、カスタムフィールドの値は&#x200B;**転送されません**。

   >[!MORELIKETHIS]
   >
   >[Web レポートでのリードまたは匿名の訪問者の表示](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
