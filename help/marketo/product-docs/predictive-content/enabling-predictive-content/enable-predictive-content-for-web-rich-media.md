---
unique-page-id: 7514956
description: サイトでWeb リッチメディアテンプレートの予測コンテンツを有効にする方法を説明します。 タイトルを個別または一括でオンにしてから、開発者用ドキュメントごとにJavaScriptを埋め込んでカスタマイズします。
title: Web リッチメディアの予測コンテンツの有効化
exl-id: 030f1dd7-8fe7-4c82-be5e-052f0a259e3c
feature: Predictive Content
TQID: https://experienceleague.adobe.com/wMtEDTeYvsyktbCKcgyvlt8PauPw7Z5uKdDHQkkV7jE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 338
ht-degree: 83%

---

# Web リッチメディアの予測コンテンツの有効化 {#enable-predictive-content-for-web-rich-media}

Web リッチメディアは、機械学習と予測分析を利用して、最も関連性の高いコンテンツで web 訪問者を引きつける機能です。 Web リッチメディアを使用すると、テキストの説明や画像を使用してコンテンツを強化し、web サイトに複数の予測コンテンツのレコメンデーションを埋め込むことができます。

>[!NOTE]
>
>予測コンテンツをテストして使用する前に、カテゴリおよびソース（電子メール、リッチメディア、バー）ごとに5つ以上のコンテンツを有効にすることをお勧めします。 コンテンツが多いほど、より良い予測結果が得られます。

>[!PREREQUISITES]
>
>予測コンテンツを有効にする前に、次の操作が必要です。
>
>* **予測コンテンツの準備**
>
>   * [メールの予測コンテンツの編集](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target="_blank"}、または
>   * [リッチメディアの予測コンテンツの編集](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target="_blank"}、または
>   * [レコメンデーションバーの予測コンテンツの編集](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target="_blank"}
>
>* [予測コンテンツのタイトルの承認](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target="_blank"}

リッチメディアのコンテンツタイトル、説明、画像を準備できたら、コンテンツピースを 1 つずつ、または複数まとめて有効にすることができます。

1. 個々のタイトルを有効にするには、タイトルをクリックしてエディターを開きます。 「**[!UICONTROL リッチメディア]**」をクリックし、「**[!UICONTROL リッチメディアでの予測コンテンツを有効にする]**」ボックスをオンにして、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2017-10-3-9-3a50-3a29.png)

1. 複数のコンテンツがある場合は、**[!UICONTROL 予測コンテンツ]**&#x200B;ページで、タイトルの横にあるチェックボックスをオンにします。

   ![](assets/image2017-10-3-10-3a0-3a42.png)

1. 「**[!UICONTROL コンテンツアクション]**」ドロップダウンをクリックし、「**[!UICONTROL Web リッチメディアを有効にする]**」を選択します。

   ![](assets/image2017-10-3-10-3a2-3a6.png)|

## JavaScript コードのカスタマイズと web サイトへの埋め込み  {#customize-the-javascript-code-and-embed-it-into-your-website}

詳しくは、[Marketo Developers サイト](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/javascriptapi/rich-media-recommendation){target="_blank"}のリッチメディアレコメンデーションテンプレートのドキュメントを参照してください。 ここでは、web サイトのテンプレートをカスタマイズする方法について説明します。

Web サイトでテンプレートを表示したい場所に JavaScript コードを貼り付けます。

**テンプレートの例**

* テンプレート 1：画像、ヘッダー、説明を含む 3 つの水平コンテンツ
* テンプレート 2：画像、ヘッダー、説明を含む 3 つの垂直コンテンツ

リッチメディアレコメンデーションテンプレート 1 の例を次に示します。

![](assets/image2015-6-1-17-3a8-3a33.png)

リッチメディアレコメンデーションテンプレート 2 の例を次に示します。

![](assets/image2015-12-20-10-3a35-3a12.png)
