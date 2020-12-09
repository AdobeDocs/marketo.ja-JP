---
unique-page-id: 1900577
description: 電子メールスクリプトトークンの作成 — Marketto Docs — 製品ドキュメント
title: 電子メールスクリプトトークンの作成
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---


# 電子メールスクリプトトークンの作成 {#create-an-email-script-token}

上級開発者は、電子メールで [Velocityスクリプト](http://velocity.apache.org/engine/1.7/user-guide.html) を使用できます。 その方法を次に示します。

1. 「 **マーケティングアクティビティ**」に移動します。

   ![](assets/ma.png)

1. 任意のプログラム(イベント、デフォルト、またはアクションなど)を検索して選択します。

   ![](assets/image2014-9-17-22-3a21-3a24.png)

1. 「 **マイトークン** 」タブで、 **** 電子メールスクリプトトークンをドラッグします。

   ![](assets/image2014-9-17-22-3a21-3a29.png)

1. 電子メールスクリプトトークンの名前を指定し、 **クリックして** 、内容を編集します。

   ![](assets/image2014-9-17-22-3a21-3a46.png)

1. 右側のツリーを使用して、 **Person、Opportunity**、 **Custom Object** Tokenをドラッグします。

   ![](assets/five-2.png)

   >[!NOTE]
   >
   >配列（オポチュニティまたはカスタムオブジェクト）にアクセスする場合、そのユーザーに関連付けられた最新10個のアイテムに制限されます。

1. スクリプトエディターにトークンをドラッグすると、トークンがchecked/activeになります。

   ![](assets/image2014-9-17-22-3a22-3a33.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >トークンを自由形式で入力する場合は、ツリー内の対応するすべてのトークンをチェック/アクティブ化する必要があります。そうしないと、プレーンテキストとして扱われ、機能しません。

1. Velocityでスクリプトを作成します。 以下に役立つリソースを示します。

   * [マーケティング担当者向け電子メールスクリプティングドキュメント](http://developers.marketo.com/email-scripting/)
   * [Velocityユーザーガイド](http://velocity.apache.org/engine/devel/user-guide.html)
   * [速度リファレンスガイド](http://velocity.apache.org/engine/devel/vtl-reference-guide.html)
   * [VelocityツールJavadoc](http://velocity.apache.org/tools/releases/2.0/javadoc/index.html)

1. スクリプトが完了したら、「 **保存**」をクリックします。

   ![](assets/image2014-9-17-22-3a23-3a1.png)

1. 「 **保存** 」をもう一度クリックします。

   ![](assets/image2014-9-17-22-3a23-3a13.png)

これで、このトークンを電子メールで使用できます。 電子メールが送信されるたびにスクリプトが実行されます。

>[!MORELIKETHIS]
>
>* [電子メ追加ールへの電子メールスクリプトトークン](add-an-email-script-token-to-your-email.md)

>



