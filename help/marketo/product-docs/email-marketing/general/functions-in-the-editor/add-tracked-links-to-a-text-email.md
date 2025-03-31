---
unique-page-id: 1900589
description: テキストメールに追跡リンクを追加する - Marketo ドキュメント - 製品ドキュメント
title: テキストメールに追跡リンクを追加する
exl-id: 10b4e029-de23-4054-83f7-b68fea68c838
feature: Email Editor
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: ht
source-wordcount: '157'
ht-degree: 100%

---

# テキストメールに追跡リンクを追加する {#add-tracked-links-to-a-text-email}

>[!PREREQUISITES]
>
>* [テキストのみのメールを作成する](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-a-text-only-email.md)
>* [メールの要素を編集する](/help/marketo/product-docs/email-marketing/general/email-editor-2/edit-elements-in-an-email.md)

Marketo では、テキストのメールリンクを追跡できます。 仕組みを見てみましょう。

1. メールを選択して、「**ドラフトを編集**」をクリックします。

![](assets/one-9.png)

1. リンクを追加する編集可能領域をダブルクリックします。

   ![](assets/two-8.png)

1. URL を二重引用符で囲んで入力します（例：`[[www.domain.com/path/page.html]]`）。

   ![](assets/three-8.png)

   >[!CAUTION]
   >
   >メールを 365 日以上前に送信し&#x200B;**、**&#x200B;過去 180 日間にそのリンクをクリックしていない場合、Marketo Engage はデータベースから URL へのルートを削除するので、リンクが破損します。 リンクを永続的にする必要がある場合は、トラッキングを使用しないでください。

1. エディターを閉じます。忘れずにドラフトを承認してください。

   ![](assets/four-6.png)

>[!NOTE]
>
>mktNoTok クラス機能は、テキストメール内の追跡可能なリンクでは機能しません。 機能するのは HTML メールの場合のみです。
