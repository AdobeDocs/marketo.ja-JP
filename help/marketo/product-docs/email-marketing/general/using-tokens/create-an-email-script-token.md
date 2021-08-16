---
unique-page-id: 1900577
description: メールスクリプトトークンを作成する — Marketo ドキュメント — 製品ドキュメント
title: メールスクリプトトークンを作成する
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '235'
ht-degree: 100%

---

# メールスクリプトトークンを作成する {#create-an-email-script-token}

上級の開発者は、メールで [Velocity スクリプト](https://velocity.apache.org/engine/1.7/user-guide.html)を使用できます。その方法を説明しましょう。

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/ma.png)

1. 任意のプログラム（イベント、デフォルト、エンゲージメントなど）を選択します。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 「**マイトークン**」タブで、**メールスクリプト**&#x200B;トークンをドラッグします。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. メールスクリプトトークンに名前を付け、**クリックして内容を編集**&#x200B;します。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 右側のツリーを使用して、**リード、商談**、または&#x200B;**カスタムオブジェクト**&#x200B;トークンをドラッグします。

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

   * [Marketo 開発者向けメールスクリプティングのドキュメント](https://developers.marketo.com/email-scripting/)
   * [Velocity ユーザーガイド](https://velocity.apache.org/engine/devel/user-guide.html)
   * [Velocity リファレンスガイド](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity ツール Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. スクリプトが完了したら、「**保存**」をクリックします。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 「**保存**」をもう 1 回クリックします。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

これで、このトークンをメールで使用できます。メールが送信されるたびにスクリプトが実行されます。

>[!MORELIKETHIS]
>
>[メールにメールスクリプトトークンを追加する](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)>
>
