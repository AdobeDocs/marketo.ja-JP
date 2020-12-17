---
unique-page-id: 1900573
description: 電子メ追加ール — Marketto Docs — 製品ドキュメント内のリンクとしてのシステムトークン
title: 電子メ追加ール内のリンクとしてのシステムトークン
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# 電子メ追加ール{#add-a-system-token-as-a-link-in-an-email}内のリンクとしてのシステムトークン

これらのシステムトークンを使用して、電子メール内の特別なリンクの位置をカスタマイズできます。

次のトークンは、電子メールまたは電子メールテンプレート内のリンクとして使用できます。

* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

>[!NOTE]
>
>これらのトークンは、アンカーリンク内でない限り&#x200B;****&#x200B;クリックできません。 また、マイトークンに&#x200B;****&#x200B;を埋め込むことはできません。

電子メールに追加する方法を次に示します。

1. 電子メールを探して選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/one-1.png)

1. 編集可能な領域内で重複を押しながらクリック

   ![](assets/two-1.png)

1. トークンを持つリンクに変換するテキストをハイライト表示し、「**リンクを挿入/編集**」ボタンをクリックします。

   ![](assets/three-1.png)

1. 「リンクURL」にトークンを入力し、「**挿入**」をクリックします。

   ![](assets/four-1.png)

   >[!TIP]
   >
   >必要なトークンをコピー/貼り付けます。**`{{system.forwardToFriendLink}}`**&#x200B;または&#x200B;**`{{system.unsubscribeLink}}`**&#x200B;または&#x200B;**`{{system.viewAsWebpageLink}}`**

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-17-22-3a12-3a17.png)

>[!NOTE]
>
>**Reminder**
>
>終了したら[メール](../../../../product-docs/email-marketing/general/creating-an-email/approve-an-email.md)を承認するのを忘れないでください。

うまくいった！ これで、システムトークンを電子メール内のリンクとして追加する方法がわかりました。