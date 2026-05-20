---
unique-page-id: 2360181
description: 匿名アクティビティとユーザーのトラッキングなど、Marketo Engageでの匿名アクティビティとユーザーのトラッキングについて説明します。 このガイドを使用して、次のステップを完了してください。
title: 匿名アクティビティとリードのトラッキング
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 90%

---

# 匿名アクティビティとリードのトラッキング {#tracking-anonymous-activity-and-people}

Marketo の[ランディングページ](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md)（または web サイト上で [Munchkin トラッキングコード](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つページ）に初めて訪問すると、Marketo は&#x200B;_匿名アクティビティ_&#x200B;を作成し、ブラウザー cookie を使用してトラックします。 識別されると、その訪問者はリードとなり、ブラウザーの Cookie に関連付けられた履歴が結合されます。

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
   * [REST API](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/leads) または [Munchkin](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) API（開発者向け）を使用して、匿名のアクティビティを既知のレコードに関連付けたとき。

   異なるデバイスやブラウザーからサイトにアクセスされることが多いので、データベース内の 1 つの名前が多くの cookie に関連付けられる場合があります。

   >[!NOTE]
   >
   >匿名レコードが新しいリードレコードまたは既存のリードレコードに結合されると、カスタムフィールドの値は&#x200B;**転送されません**。

   >[!MORELIKETHIS]
   >
   >[Web レポートでのリードまたは匿名の訪問者の表示](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
