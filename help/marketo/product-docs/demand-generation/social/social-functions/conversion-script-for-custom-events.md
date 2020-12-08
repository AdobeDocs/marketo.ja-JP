---
unique-page-id: 2950561
description: カスタムイベント- Marketto Docs — 製品ドキュメントのコンバージョンスクリプト
title: カスタムイベントのコンバージョンスクリプト
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---


# カスタムイベントのコンバージョンスクリプト {#conversion-script-for-custom-events}

参照オファーを作成する際に、受渡目標を定義します。 目標に向けてカウントするアクションが独自のWebページ上の特定のイベントである場合、コンバージョンスクリプトを使用してJavaScript APIを呼び出すことができます。

## 変換スクリプトの取得 {#retrieve-the-conversion-script}

1. 照会オファーエディターで「 **オファーの詳細** 」をクリックし、「受渡目標 **」ドロップダウンから「** 顧客JavaScriptイベント」を選択します。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 灰色のボックスの先頭のスクリプトをコピーし、タグ内のWebページに配置し `<body>` ます。 下部のスクリプトはタグ内に配置し `<header>` ます。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >両方のスクリプトをコピーして貼り付けるのは、マーケティング担当者以外のWebサイトを対象とする場合に限ります。

## ローダスクリプトの取得 {#retrieve-the-loader-script}

1. ツリーから参照オファーを選択し、「参照オファーのアクション **」および「** 埋め込みコード ****」をクリックします。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. 「 **ヘッダーコード** 」を右クリックし、Webページのヘッダーに挿入します。 次に、 **本文コードに対しても同じ操作を行います**。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Webページへのスクリプトの貼り付け {#pasting-the-scripts-onto-your-webpage}

変換スクリプトを、bodyとheaderのHTMLに貼り付けます。 次に、ローダースクリプトをbodyとheaderのHTMLに配置します。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 変換スクリプトの接続 {#connecting-the-conversion-script}

目標の完了をトリガーするページ要素の特定のHTML IDを使用するJavaScript関数を記述する場所です。 次に例を示します。

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

この例では、Webページに「#myButtonId」というIDのボタンがあります。 そのボタンをクリックすると、その人は目標を完了したと登録されます。

すごい！ Webサイトで、Marketoを使用したカスタムソーシャルプロモーションの目標を捕捉するようになりました。

>[!NOTE]
>
>**関連記事**
>
>* [照会オファーの目標の指定](../../../../product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [照会オファーの作成](../../../../product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [WebサイトにSocialを導入する](deploy-social-on-your-website.md)

