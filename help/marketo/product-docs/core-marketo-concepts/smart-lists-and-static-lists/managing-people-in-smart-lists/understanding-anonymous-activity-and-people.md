---
unique-page-id: 1147322
description: Marketoの匿名アクティビティとユーザーについて説明します。 コンバージョン前に匿名の訪問者がどのように追跡されるのかを把握できます。
title: 匿名アクティビティとリードについて
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
TQID: https://experienceleague.adobe.com/avWmJKBGktOEseVl3uIYB9Bp19Rq3HQgo98gKJFDtIc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 271
ht-degree: 87%

---

# 匿名アクティビティとリードについて {#understanding-anonymous-activity-and-people}

Marketo のランディングページ（または web サイト上で [Munchkin トラッキングコード](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}を持つページ）に初めて訪問すると、Marketo は&#x200B;*匿名アクティビティ*&#x200B;を作成し、ブラウザー cookie を使用してトラックします。 識別されると、人物になり、ブラウザーCookieに関連付けられた履歴が結合されます。

>[!IMPORTANT]
>
>ベータ版機能である **[!DNL Munchkin]V2 Anonymous Replay Activity on Known** を有効にすると、匿名リードのプロモーションによってトリガーされたキャンペーンが、匿名リードが既知のレコードに正常に結合された後に常に再生されるようになります。 その結果、再生されたキャンペーンのデータ値の変更ステップで変更されたカスタムフィールドは、既知のレコードに保持されます。

**匿名**&#x200B;アクティビティは、次の場合に作成されます。

* 初めて Marketo のランディングページにアクセスしたとき。
* [Munchkin トラッキング](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}を持つサイトのページを訪問したとき。
* Marketo メールの「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}」リンクをクリックしたとき。

>[!NOTE]
>
>Marketo メールの他のリンクとは異なり、「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}」は、メールクリックとしてはトラックされません。

匿名アクティビティは、次の場合に、新規または既存のユーザに結合されます。

* [Marketo メール内のリンク](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}をクリックしたとき。
* Marketo の[フォーム](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}に入力したとき。
* [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} または [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API（開発者向け）を使用して、匿名のリードを既知のレコードに関連付けたとき。

異なるデバイスやブラウザーからサイトにアクセスされることが多いので、データベース内の 1 つの名前が多くの cookie に関連付けられる場合があります。

>[!NOTE]
>
>匿名レコードが新しいリードレコードまたは既存のリードレコードに結合されると、カスタムフィールドの値は&#x200B;*転送されません*。
