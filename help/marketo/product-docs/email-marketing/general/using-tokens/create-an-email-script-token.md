---
unique-page-id: 1900577
description: メールスクリプトトークンを作成する — Marketo ドキュメント — 製品ドキュメント
title: メールスクリプトトークンを作成する
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 88%

---

# メールスクリプトトークンを作成する {#create-an-email-script-token}

上級の開発者は、メールで [Velocity スクリプト](https://velocity.apache.org/engine/1.7/user-guide.html)を使用できます。その方法を説明しましょう。

1. 「**[!UICONTROL マーケティングアクティビティ]**」に移動します。

   ![](assets/ma.png)

1. 任意のプログラム（イベント、デフォルト、エンゲージメントなど）を選択します。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 「**[!UICONTROL マイトークン]**」タブで、**[!UICONTROL メールスクリプト]**&#x200B;トークンをドラッグします。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. メールスクリプトトークンに名前を付け、そのコンテンツを **[!UICONTROL クリックして編集]** します。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 右側のツリーを使用して、**[!UICONTROL Person]**、**[!UICONTROL Opportunity]**、**[!UICONTROL Custom Object]** トークンをドラッグします。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >配列（商談またはカスタムオブジェクト）にアクセスする場合、そのリードに関連付けられた最新の 10 個の項目に制限されます。

1. トークンをスクリプトエディターにドラッグすると、トークンがチェックされ、アクティブになります。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >トークンを自由形式で入力する場合は、ツリー内の対応するトークンすべてにチェックを付ける（つまり、有効化する）のを忘れないようにしてください。そうしないと、プレーンテキストとして処理され、正しく機能しません。

1. Velocity でスクリプトを作成します。以下に、役立つリソースを示します。

   * [Marketo 開発者向けメールスクリプティングのドキュメント](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/email-scripting)
   * [Velocity ユーザーガイド](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity リファレンスガイド](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity ツール Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. スクリプトが完了したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 「**[!UICONTROL 保存]**」をもう 1 回クリックします。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

これで、このトークンをメールで使用できます。メールが送信されるたびにスクリプトが実行されます。

>[!MORELIKETHIS]
>
>[メールへのメールスクリプトトークンの追加](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
