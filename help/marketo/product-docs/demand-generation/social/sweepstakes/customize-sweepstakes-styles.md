---
unique-page-id: 2359807
description: 懸賞のスタイルのカスタマイズ —Marketoドキュメント — 製品ドキュメント
title: 懸賞のスタイルのカスタマイズ
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# 懸賞のスタイルのカスタマイズ{#customize-sweepstakes-styles}

[懸賞](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)を作成するとき、ランディングページ上での懸賞の外観をカスタマイズできます。

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。  詳細は、営業取引先責任者にお問い合わせください。

1. **マーケティングアクティビティ**&#x200B;に移動します。

![](assets/login-marketing-activities-1.png)

1. 懸賞を選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. Sweepstakesエディターで、**アプリ設定**/**外観**&#x200B;に移動します。

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. サインアップボタンのテキストと進行状況リンクを編集します。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. カスタマイズする要素ごとに、カスタムCSSプロパティを入力します。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   **Enter Button**のCSSの例：
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   **入力ボタン**の画像の例：
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >テキストが含まれる画像を使用する場合は、上の「テキスト」の下の「**入力ボタン**」フィールドからテキストを削除するようにしてください。

1. 変更を行うたびに、結果が表示と編集プレビューに表示されます。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >古いバージョンを含む様々なブラウザーでボタンをテストします。

   >[!MORELIKETHIS]
   >
   >次の手順は、[サインアップメールと受渡通知メールを懸賞へ追加](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md)することです。
