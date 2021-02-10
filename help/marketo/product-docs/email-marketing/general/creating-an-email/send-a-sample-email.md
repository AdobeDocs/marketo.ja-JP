---
unique-page-id: 1147352
description: サンプルの電子メール — Marketto Docs — 製品ドキュメントの送信
title: サンプル電子メールの送信
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# サンプルの電子メールの送信{#send-a-sample-email}

電子メールのサンプルを簡単に送信できます。 動的なコンテンツの電子メールを送信するには、「[動的なコンテンツを含む電子メールのプレビュー](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md)」を参照してください。

>[!NOTE]
>
>サンプル電子メールを送信するには、**データベースへのアクセス — 単一フローアクションの実行**&#x200B;権限が必要です。

## サンプルの電子メールの送信{#send-a-sample-email-1}

1. 電子メールを探して選択します。 「**電子メールアクション**」ドロップダウンをクリックし、「**サンプルを送信**」を選択します。\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >マイトークンは、電子メールのプログラムに適した値に解決されます。

1. 配信の電子メールアドレスを入力し、「**送信**」をクリックします。

   ![](assets/two.png)

   >[!NOTE]
   >
   >複数の電子メールアドレスを入力する場合は、コンマで区切ります。

   >[!TIP]
   >
   >トークンを特定のユーザーとして解決する場合は、手順2の&#x200B;**ユーザードロップダウン**&#x200B;でそのユーザーを選択します。

## {#send-a-sample-email-while-editing}の編集中にサンプル電子メールを送信

1. 電子メールを探し、その電子メールを選択して、「**ドラフトを編集**」タブをクリックします。

   ![](assets/three-281-29.jpg)

1. 「**電子メールアクション**」をクリックし、「**サンプルを送信**」を選択します。

   ![](assets/four.png)

1. 配信の電子メールアドレスを入力し、「**送信**」をクリックします。

   ![](assets/two.png)

   >[!NOTE]
   >
   >トリガーフィールドは、[emailスクリプティング](https://developers.marketo.com/documentation/velocity-script/)を使用する場合にのみ適用できます。

## セグメントに基づくサンプル電子メールの送信{#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[電子メールにセグメントを適用します](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md)。

1. 電子メールを探し、その電子メールを選択して、「**ドラフトを編集**」タブをクリックします。

   ![](assets/three-281-29.jpg)

1. **プレビュー**&#x200B;をクリックします。

   ![](assets/1.png)

1. 「**表示基準**」ドロップダウンをクリックし、「**セグメント化**」を選択します。

   ![](assets/2.png)

1. 使用可能なセグメントを含むドロップダウンが表示されます。 クリックし、目的のレポートを選択します。

   ![](assets/3.png)

1. 矢印を使用して、オプションをスクロールします（この場合は、件名行を動的に変更しました）。

   ![](assets/4.png)

1. 「**サンプルを送信**」をクリックして、実行中のセグメントのテスト電子メールを受信します。

   ![](assets/5.png)

   >[!TIP]
   >
   >セグメントに基づいたサンプルの電子メールを電子メールの編集モードで送信することもできます。 「**電子メールアクション**」ドロップダウンをクリックし、「**サンプルを送信**」を選択して、セグメントを選択します。

キャンペーンを起動する前にコンテンツをサンプリングすることは非常に重要です。 2度、1回切れ！
