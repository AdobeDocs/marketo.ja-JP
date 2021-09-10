---
unique-page-id: 2950561
description: カスタムイベントのコンバージョンスクリプト — Marketo ドキュメント — 製品ドキュメント
title: カスタムイベントのコンバージョンスクリプト
exl-id: 202b7e66-af83-42fd-8067-a5808eba7c32
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '276'
ht-degree: 100%

---

# カスタムイベントのコンバージョンスクリプト {#conversion-script-for-custom-events}

紹介オファーを作成する際に、達成目標を定義します。目標に対するアクションが、独自の Web ページ上の特定のイベントである場合は、コンバージョンスクリプトを使用して JavaScript API を呼び出すことができます。

## コンバージョンスクリプトの取得 {#retrieve-the-conversion-script}

1. 紹介オファーエディター内で、「**オファーの詳細**」をクリックして、達成目標ドロップダウンから&#x200B;**カスタム Javascript イベント**&#x200B;を選択します。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 灰色のボックスの上部のスクリプトをコピーして、Web ページの `<body>` タグ内に配置します。下部のスクリプトは、`<header>` タグ内に配置します。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >Marketo 以外の Web サイトの場合は、忘れずに両方のスクリプトをコピー＆ペーストしてください。

## ローダースクリプトの取得 {#retrieve-the-loader-script}

1. ツリーから紹介オファーを選択して、「**紹介オファーアクション**」と「**埋め込みコード**」をクリックします。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. **ヘッダーコード**&#x200B;を右クリックして、Web ページのヘッダーに挿入します。次に、**本文コード**&#x200B;に対しても、同じ操作を行います。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Web ページへのスクリプトの貼り付け {#pasting-the-scripts-onto-your-webpage}

コンバージョンスクリプトを HTML の本文とヘッダーに貼り付けます。次に、ローダースクリプトを HTML の本文とヘッダーに配置します。

![](assets/image2015-4-20-21-3a0-3a16.png)

## コンバージョンスクリプトの接続 {#connecting-the-conversion-script}

ここでは、目標の完了をトリガーするページ要素の特定の HTML ID を使用する JavaScript 関数を記述します。例：

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

この例では、Web ページに「#myButtonId」という ID のボタンがあります。そのボタンをクリックすると、その担当者が目標を完了したと登録されます。

これで完了です。これで、Web サイトが Marketo を使用したカスタムのソーシャルプロモーション目標をキャプチャします。

>[!MORELIKETHIS]
>
>* [紹介オファーの目標の指定](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [紹介オファーの作成](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [Web サイトへのソーシャルのデプロイ](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

