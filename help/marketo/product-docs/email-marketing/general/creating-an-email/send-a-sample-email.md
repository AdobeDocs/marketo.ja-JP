---
unique-page-id: 1147352
description: サンプルメールを送信する - Marketo ドキュメント - 製品ドキュメント
title: サンプルメールを送信する
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
source-git-commit: 1586b71ec9f9c4f8abc4fd9a3277d5a5f5b88080
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 83%

---

# サンプルメールを送信する {#send-a-sample-email}

メールのサンプルを迅速かつ簡単に送信できます。動的コンテンツを含むメールを送信するには、「[動的コンテンツを使ったメールをプレビューする](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)」を参照してください。

>[!NOTE]
>
>サンプルメールの送信には、**データベースにアクセス - シングルフローアクションの実行**&#x200B;権限が必要です。

## サンプルメールを送信する {#send-a-sample-email-1}

1. メールを選択します。**メールアクション**&#x200B;ドロップダウンをクリックし、「**サンプルの送信**」を選択します。\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >マイトークンは、メールのプログラムに適した値に解決されます。

1. 配信する E メールアドレスを 1 つ以上入力します。 複数の電子メールアドレスの場合は、コンマで区切ります。 クリック **送信** 完了したら、

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >複数の電子メールアドレスを入力すると、すべての受信者に表示されます。 最初に入力した受信者はメイン受信者で、その後に続く E メールアドレスは CC 受信者です。

   >[!TIP]
   >
   >トークンを特定のリードとして解決したい場合は、手順 2 の&#x200B;**リードドロップダウン**&#x200B;メニューで値を選択します。

## 編集中にサンプルメールを送信する {#send-a-sample-email-while-editing}

1. メールを選択し、「**ドラフトの編集**」をクリックします。

   ![](assets/three-281-29.jpg)

1. 「**メールアクション**」をクリックして、「**サンプルの送信**」を選択します。

   ![](assets/four.png)

1. 配信用のメールアドレスを入力して「**送信**」をクリックします。

   ![](assets/two.png)

   >[!NOTE]
   >
   >「トリガー」フィールドは、[メールスクリプティング](https://developers.marketo.com/documentation/velocity-script/)を使用する場合にのみ適用できます。

## セグメントに基づくサンプルメールの送信 {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[メールにセグメント化を適用します](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md)。

1. メールを選択し、「**ドラフトの編集**」をクリックします。

   ![](assets/three-281-29.jpg)

1. 「**プレビュー**」をクリックします。

   ![](assets/1.png)

1. **閲覧方法**&#x200B;ドロップダウンをクリックし、「**セグメント化**」を選択します。

   ![](assets/2.png)

1. 使用可能なセグメント化を含むドロップダウンが表示されます。それをクリックし、目的のものを選択します。

   ![](assets/3.png)

1. 矢印を使用して、オプションをスクロールします（この場合は、件名行を動的に変更します）。

   ![](assets/4.png)

1. 「**サンプルの送信**」をクリックすると、実行中のセグメントのテスト用メールが届きます。

   ![](assets/5.png)

   >[!TIP]
   >
   >また、メールの編集モードでセグメントに基づいてサンプルメールを送信することもできます。**メールアクション**&#x200B;ドロップダウンをクリックし、「**サンプルの送信**」を選択して、セグメントを選択します。

キャンペーンを開始する前にコンテンツのサンプルを確認することは非常に重要です。実行に移す前に、念には念を入れましょう。
