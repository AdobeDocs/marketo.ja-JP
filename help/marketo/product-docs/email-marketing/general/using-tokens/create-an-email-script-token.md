---
unique-page-id: 1900577
description: メールスクリプトトークンの作成方法を説明します。 メールに動的な値を出力するカスタムトークンを定義できます。
title: メールスクリプトトークンを作成する
exl-id: c7f8c3e0-6d64-4115-b9b6-261576360ba1
feature: Tokens
TQID: https://experienceleague.adobe.com/3FbkNKaOjEX--zXCOC1EHLEVr5ChimEOJTROMY0bHmc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 87%

---

# メールスクリプトトークンを作成する {#create-an-email-script-token}

上級の開発者は、メールで [Velocity スクリプト](https://velocity.apache.org/engine/1.7/user-guide.html)を使用できます。 その方法を説明しましょう。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/ma.png)

1. 任意のプログラム（イベント、デフォルト、エンゲージメントなど）を選択します。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 「**[!UICONTROL マイトークン]**」タブで、**[!UICONTROL メールスクリプト]**&#x200B;トークンをドラッグします。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. メールスクリプトトークンに名前を付け、**[!UICONTROL クリックして内容を編集]**&#x200B;します。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 右側のツリーを使用して、**[!UICONTROL リード]**、**[!UICONTROL 商談]**、または&#x200B;**[!UICONTROL カスタムオブジェクト]**&#x200B;トークンをドラッグします。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >配列（商談またはカスタムオブジェクト）にアクセスする場合、そのリードに関連付けられた最新の 10 個の項目に制限されます。

1. トークンをスクリプトエディターにドラッグすると、トークンがチェックされ、アクティブになります。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >トークンを自由形式で入力する場合は、ツリー内の対応するトークンすべてにチェックを付ける（つまり、有効化する）のを忘れないようにしてください。そうしないと、プレーンテキストとして処理され、正しく機能しません。

1. Velocity でスクリプトを作成します。 以下に、役立つリソースを示します。

   * [Marketo Developers メールスクリプティングドキュメント](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/email-scripting)
   * [Velocity ユーザーガイド](https://velocity.apache.org/engine/devel/user-guide.html)
   * [速度リファレンスガイド](https://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [Velocity Tools Javadoc](https://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. スクリプトが完了したら、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 「**[!UICONTROL 保存]**」をもう 1 回クリックします。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

これで、このトークンをメールで使用できます。 メールが送信されるたびにスクリプトが実行されます。

>[!MORELIKETHIS]
>
>[メールへのメールスクリプトトークンの追加](/help/marketo/product-docs/email-marketing/general/using-tokens/add-an-email-script-token-to-your-email.md)
