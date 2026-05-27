---
unique-page-id: 1900573
description: メールにシステムトークンをリンクとして追加する方法を説明します。 リンク URLでトークンを使用して、購読解除またはその他の動的リンクを行います。
title: メールにシステムトークンをリンクとして追加する
exl-id: 9156be24-18ae-44ea-96e5-a6257ff29b46
feature: Tokens
TQID: https://experienceleague.adobe.com/UjNwoeeRWyGrPUCMV--3StSZcbY-fxSj3a5wrm60oL4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 224
ht-degree: 80%

---

# メールにシステムトークンをリンクとして追加する {#add-a-system-token-as-a-link-in-an-email}

これらのシステムトークンを使用して、メール内の特別なリンクの位置をカスタマイズできます。

次のトークンは、メールまたはメールテンプレート内のリンクとして使用できます。

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>これらのトークンは、アンカーリンク内にない限り、クリック&#x200B;**できません**。 また、マイトークンに埋め込むことも&#x200B;**できません**。

メールに追加する方法を次に示します。

1. メールを探して選択し、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/one-1.png)

1. 編集可能な領域をダブルクリックします。

   ![](assets/two-1.png)

1. トークンを含むリンクに変換するテキストをハイライト表示し、「**[!UICONTROL リンクを挿入／編集]**」ボタンをクリックします。

   ![](assets/three-1.png)

1. 「リンク URL」にトークンを入力し、「**[!UICONTROL 挿入]**」をクリックします。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >目的のトークン（**`{{system.forwardToFriendLink}}`**、**`{{system.unsubscribeLink}}`**、**`{{system.viewAsWebpageLink}}`** のいずれか）をコピー＆ペーストします。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!IMPORTANT]
>
>このアプローチを使用して「viewAsWebpageLink」システムトークンを追加する場合は、トークンを使用して&#x200B;**not**&#x200B;上書きできます。 代わりに、[メールに「Web ページとして表示」リンクを追加する](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)アプローチを使用すれば、トークンを使用して「viewAsWebPageLink」を上書きできます。

>[!NOTE]
>
>完了したら、忘れずに[メールを承認](/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md)してください。

これで完了です。 システムトークンをリンクとしてメールに追加する方法がわかりました。
