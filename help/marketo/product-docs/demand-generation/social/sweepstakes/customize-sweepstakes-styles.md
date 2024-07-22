---
unique-page-id: 2359807
description: 懸賞のスタイルのカスタマイズ - Marketo ドキュメント - 製品ドキュメント
title: 懸賞スタイルのカスタマイズ
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 100%

---

# 懸賞スタイルのカスタマイズ {#customize-sweepstakes-styles}

[懸賞を作成する](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md)場合、ランディングページでの表示をカスタマイズできます。

>[!AVAILABILITY]
>
>すべての Marketo Engage ユーザがこの機能を購入しているわけではありません。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

1. 「**マーケティングアクティビティ**」に移動します。

![](assets/login-marketing-activities-1.png)

1. 懸賞を選択し、「**ドラフトを編集**」をクリックします。

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. 懸賞エディターで、**アプリ設定**／**表示方法**&#x200B;に移動します。

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. 新規登録ボタンのテキストと進行状況リンクを編集します。

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. カスタマイズする各要素に対して、カスタム CSS プロパティを入力します。

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   **入力ボタン**の CSS の例：
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   **入力ボタン**の画像の例：
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >テキストが含まれている画像を使用する場合は、上の「テキスト」の下の「**入力ボタン**&#x200B;フィールドからテキストを削除することを忘れないでください。

1. 変更を加えるたびに、結果が表示と編集のプレビューに表示されます。

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >古いバージョンも含めた複数の異なるブラウザーでボタンをテストします。

   >[!MORELIKETHIS]
   >
   >次に、[懸賞に新規登録メールと達成メール](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md)を追加します。
