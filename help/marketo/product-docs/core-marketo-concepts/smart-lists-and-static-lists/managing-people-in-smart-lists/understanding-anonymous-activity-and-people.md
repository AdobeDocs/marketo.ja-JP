---
unique-page-id: 1147322
description: 匿名アクティビティとリードについて - Marketo ドキュメント - 製品ドキュメント
title: 匿名アクティビティとリードについて
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 100%

---

# 匿名アクティビティとリードについて {#understanding-anonymous-activity-and-people}

Marketo のランディングページ（または web サイト上で [Munchkin トラッキングコード](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つページ）に初めて訪問すると、Marketo は&#x200B;_匿名アクティビティ_&#x200B;を作成し、ブラウザー cookie を使用してトラックします。識別されると、その訪問者はリードとなり、ブラウザーの Cookie に関連付けられた履歴が結合されます。

>[!IMPORTANT]
>
>ベータ版機能である **Munchkin V2 Anonymous Replay Activity on Known** を有効にすると、匿名リードのプロモーションによってトリガーされたキャンペーンが、匿名リードが既知のレコードに正常にマージされた後に常に再生されるようになります。その結果、再生されたキャンペーンのデータ値の変更ステップで変更されたカスタムフィールドは、既知のレコードに保持されます。

**匿名**&#x200B;アクティビティは、次の場合に作成されます。

* 初めて Marketo のランディングページにアクセスしたとき。
* [Munchkin トラッキング](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)を持つサイトのページを訪問したとき。
* Marketo メールの「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」リンクをクリックしたとき。

>[!NOTE]
>
>Marketo メールの他のリンクとは異なり、「[Web ページとして表示](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)」は、メールクリックとしてはトラックされません。

匿名アクティビティは、次の場合に、新規または既存のユーザに結合されます。

* [Marketo メール内のリンク](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)をクリックしたとき。
* Marketo の[フォーム](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)に入力したとき。
* [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) または [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API（開発者向け）を使用して、匿名のリードを既知のレコードに関連付けたとき。

異なるデバイスやブラウザーからサイトにアクセスされることが多いので、データベース内の 1 つの名前が多くの cookie に関連付けられる場合があります。

>[!NOTE]
>
>匿名レコードが新しいリードレコードまたは既存のリードレコードに結合されると、カスタムフィールドの値は&#x200B;**転送されません**。
