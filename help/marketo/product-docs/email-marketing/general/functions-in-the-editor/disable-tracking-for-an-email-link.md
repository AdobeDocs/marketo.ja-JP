---
unique-page-id: 1900579
description: メールリンクのトラッキングを無効にする — Marketo ドキュメント — 製品ドキュメント
title: メールリンクのトラッキングを無効にする
exl-id: 841ef605-1664-4457-bc83-50bbe5d44853
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 97%

---

# メールリンクのトラッキングを無効にする {#disable-tracking-for-an-email-link}

場合によっては、メールのリンクで **Marketo の URL トラッキング**&#x200B;機能を有効にしたくないことがあります。 この情報は、表示先ページで URL パラメーターをサポートしていないためにページリンクエラーになる場合などに役立ちます。

また、メールを 365 日以上前に送信し&#x200B;**、**&#x200B;過去 180 日間にそのリンクをクリックしていない場合、Marketo Engage はデータベースから URL へのルートを削除するので、リンクが破損します。 そのため、リンクを永続的にする必要がある場合は、トラッキングを無効にする必要があります。

1. メールを選択して、「**[!UICONTROL ドラフトを編集]**」をクリックします。

   ![](assets/one-7.png)

1. リンクを含む編集可能なセクションをダブルクリックします。

   ![](assets/two-6.png)

1. 問題のリンクをクリックして、「**リンクの挿入／編集**」ボタンをクリックします。

   ![](assets/three-6.png)

1. リンクの編集ポップアップで、「**[!UICONTROL リンクの追跡]**」チェックボックスをオフにします。

   ![](assets/four-4.png)

1. **[!UICONTROL Include mkt_tok] ボックス** が消えます。 「**[!UICONTROL 適用]**」をクリックします。

   ![](assets/five-3.png)

   >[!TIP]
   >
   >**Include mkt_tok** のみをオフにしてもリンクのトラッキングは可能ですが、リダイレクト後、宛先 URL に mkt_tok クエリ文字列パラメーターは含まれません。 このパラメーターは、リードのアクティビティを適切にトラッキングするために（リードがメールを登録解除した場合など）、Marketo のランディングページと Munchkin で使用されます。 パラメーターが存在することが原因で Web サイトに変な動作が発生していない限り、この機能の使用は避けてください。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-17-22-3a25-3a20.png)

   >[!CAUTION]
   >
   >メールテンプレート内のリンクや[テキストバージョン](/help/marketo/product-docs/email-marketing/general/creating-an-email/edit-the-text-version-of-an-email.md){target="_blank"}のメールのクリックトラッキングを無効にする場合は、文字列の末尾ではなく&#x200B;*先頭*&#x200B;に `mktNoTrack` を追加します（例：`<a class="mktNoTrack" href="https://www.mywebsite.com">This link does not have tracking</a>`）。そうしないと、リンクが表示されなくなる可能性があります。上記のコードの実装に関するヘルプが必要な場合は、web 開発者にお問い合わせください。
