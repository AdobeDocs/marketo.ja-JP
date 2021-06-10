---
unique-page-id: 1900573
description: システムトークンを電子メールにリンクとして追加する — Marketoドキュメント — 製品ドキュメント
title: システムトークンを電子メールのリンクとして追加
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
source-git-commit: 65caed388ac33fc9f3142102343fe43ebc186e6e
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# 電子メール{#add-a-system-token-as-a-link-in-an-email}にシステムトークンをリンクとして追加する

これらのシステムトークンを使用して、Eメール内の特別なリンクの位置をカスタマイズできます。

次のトークンは、EメールまたはEメールテンプレート内のリンクとして使用できます。

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>これらのトークンは、アンカーリンク内にない限り、クリックできません。**** また、マイトークンに&#x200B;**埋め込むことはできません**。

Eメールに追加する方法を次に示します。

1. 電子メールを探して選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/one-1.png)

1. 編集可能な領域をダブルクリックします。

   ![](assets/two-1.png)

1. トークンを含むリンクに変換するテキストをハイライト表示し、「**リンクを挿入/編集**」ボタンをクリックします。

   ![](assets/three-1.png)

1. 「リンクURL 」にトークンを入力し、「**挿入**」をクリックします。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >目的のトークンをコピー/貼り付けます。**`{{system.forwardToFriendLink}}`**、**`{{system.unsubscribeLink}}`**、**`{{system.viewAsWebpageLink}}`**&#x200B;のいずれか

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>この方法を使用して「viewAsWebpageLink」システムトークンを追加する場合、トークンを使用して&#x200B;**上書きできません**。 代わりに、[Add a View as Web Page Link to an Email](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)アプローチを使用して、トークンを使用して「viewAsWebPageLink」を上書きできます。

>[!NOTE]
>
>完了したら、[電子メール](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)を承認することを忘れないでください。

うまくいった！ これで、システムトークンをリンクとしてEメールに追加する方法がわかりました。
