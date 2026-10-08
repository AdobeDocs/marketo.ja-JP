---
unique-page-id: 1900579
description: 特定のメールリンクのトラッキングを無効にする方法について説明します。 プライバシーまたはリダイレクト URLに必要な場合は、クリックトラッキングをオフにします。
title: メールリンクのトラッキングを無効にする
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/q3ADow5Tqt-k37k-joN6qGPAPiS8KRkFNUyeR8osJ8Y'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 86%
---
# メールリンクのトラッキングを無効にする {#disable-tracking-for-an-email-link}

場合によっては、メールのリンクで **Marketo の URL トラッキング**&#x200B;機能を有効にしたくないことがあります。 これは、宛先ページが URL パラメーターをサポートしておらず、リンク切れになる可能性がある場合などに役立ちます。&#x200B;

また、メールを 365 日以上前に送信し&#x200B;**、**&#x200B;過去 180 日間にそのリンクをクリックしていない場合、Marketo Engage はデータベースから URL へのルートを削除するので、リンクが破損します。 そのため、リンクを永続的にする必要がある場合は、トラッキングを無効にする必要があります。

1. メールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/one-7.png)

1. リンクを含む編集可能なセクションをダブルクリックします。

   ![](assets/two-6.png)

1. 問題のリンクをクリックして、「**リンクの挿入／編集**」ボタンをクリックします。

   ![](assets/three-6.png)

1. リンクの編集ポップアップで、「**[!UICONTROL リンクの追跡]**」チェックボックスをオフにします。

   ![](assets/four-4.png)

1. **[!UICONTROL Include mkt_tok] チェックボックス**&#x200B;が消えます。 「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >**Include mkt_tok** のみをオフにしてもリンクのトラッキングは可能ですが、リダイレクト後、宛先 URL に mkt_tok クエリ文字列パラメーターは含まれません。 このパラメーターは、リードのアクティビティを適切にトラッキングするために（リードがメールを登録解除した場合など）、Marketo のランディングページと Munchkin で使用されます。 パラメーターが存在するため、web サイトで奇妙な動作が表示されない限り、この機能を使用しないでください。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >メールテンプレート内のリンクや[テキストバージョン](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"}のメールのクリックトラッキングを無効にする場合は、文字列の末尾ではなく&#x200B;*先頭*&#x200B;に `mktNoTrack` を追加します（例：`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`）。 そうしないと、リンクが表示されなくなる可能性があります。 上記のコードを実装する際にヘルプが必要な場合は、web 開発者にお問い合わせください。
