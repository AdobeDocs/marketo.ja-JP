---
unique-page-id: 2950561
description: カスタムイベント- Marketto Docs — 製品ドキュメントのコンバージョンスクリプト
title: カスタムイベントのコンバージョンスクリプト
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# カスタムイベントの変換スクリプト{#conversion-script-for-custom-events}

参照オファーを作成する際に、受渡目標を定義します。 目標に向けてカウントするアクションが独自のWebページ上の特定のイベントである場合、コンバージョンスクリプトを使用してJavaScript APIを呼び出すことができます。

## 変換スクリプトを取得{#retrieve-the-conversion-script}

1. 参照オファーエディターで「**オファーの詳細**」をクリックし、「受渡目標」ドロップダウンから「**お客様のJavaScriptイベント**」を選択します。

   ![](assets/image2015-4-20-17-3a22-3a15.png)

1. 灰色のボックスの先頭のスクリプトをコピーし、`<body>`タグ内のWebページに配置します。 下部のスクリプトは`<header>`タグ内に配置します。

   ![](assets/image2015-4-20-17-3a29-3a7.png)

   >[!NOTE]
   >
   >両方のスクリプトをコピーして貼り付けるのは、マーケティング担当者以外のWebサイトを対象とする場合に限ります。

## ローダスクリプト{#retrieve-the-loader-script}を取得します

1. ツリーから参照オファーを選択し、**参照オファーの操作**&#x200B;と&#x200B;**埋め込みコード**&#x200B;をクリックします。

   ![](assets/image2015-4-20-17-3a34-3a46.png)

1. **ヘッダーコード**&#x200B;を右クリックし、Webページのヘッダーに挿入します。 次に、**ボディコード**&#x200B;に対しても同じようにします。

   ![](assets/image2015-4-20-20-3a49-3a19.png)

## Webページへのスクリプトの貼り付け{#pasting-the-scripts-onto-your-webpage}

変換スクリプトを、bodyとheaderのHTMLに貼り付けます。 次に、ローダースクリプトをbodyとheaderのHTMLに配置します。

![](assets/image2015-4-20-21-3a0-3a16.png)

## 変換スクリプトの接続{#connecting-the-conversion-script}

ここで、トリガー目標を完了するページ要素の特定のHTML IDを使用するJavaScript関数を記述します。 次に例を示します。

`<pre><em><!-- Referral offer conversion script --></em> <script> cf_scripts.afterload(function (){ jQuery("#myButtonId").click(function (){ CF.insight.conversion(); }); }); </script></pre>` `<pre>`

この例では、Webページに「#myButtonId」というIDのボタンがあります。 そのボタンをクリックすると、その人は目標を完了したと登録されます。

すごい！ Webサイトで、Marketoを使用したカスタムソーシャルプロモーションの目標を捕捉するようになりました。

>[!MORELIKETHIS]
>
>* [照会オファーの目標の指定](/help/marketo/product-docs/demand-generation/social/referral-offers/specify-goal-for-referral-offer.md)
>* [照会オファーの作成](/help/marketo/product-docs/demand-generation/social/referral-offers/create-a-referral-offer.md)
>* [WebサイトにSocialを導入する](/help/marketo/product-docs/demand-generation/social/social-functions/deploy-social-on-your-website.md)

