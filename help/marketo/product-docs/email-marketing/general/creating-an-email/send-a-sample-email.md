---
unique-page-id: 1147352
description: サンプルメールを送信する - Marketo ドキュメント - 製品ドキュメント
title: サンプルメールを送信する
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '289'
ht-degree: 100%

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

1. 配信用のメールアドレスを入力して「**送信**」をクリックします。

   ![](assets/two.png)

   >[!NOTE]
   >
   >複数のメールアドレスを入力する場合は、コンマで区切ります。

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
