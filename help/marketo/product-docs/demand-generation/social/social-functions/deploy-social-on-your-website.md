---
unique-page-id: 2950524
description: Web サイトへのソーシャルのデプロイ — Marketo ドキュメント — 製品ドキュメント
title: Web サイトへのソーシャルのデプロイ
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 6c3f803104c550227aec25376778147ff92aaab9
workflow-type: ht
source-wordcount: '264'
ht-degree: 100%

---

# Web サイトへのソーシャルのデプロイ {#deploy-social-on-your-website}

ソーシャルアプリを Marketo 以外のページに埋め込みます。

>[!IMPORTANT]
>
>2024年7月31日（PT）に、この機能を廃止するプロセスを開始しました。新しいアセットは作成できなくなりました。既存のアセットは、2025年1月31日（PT）まで引き続き機能します。[詳細情報](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>すべての Marketo Engage ユーザがこの機能を購入しているわけではありません。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

オーディエンスを魅了し、誰もがソーシャルネットワーク上のより大きな会話に参加できるように、ソーシャルアプリを独自の Web サイトにデプロイできます。ユーザーがソーシャルネットワーク上でプロモーションやコンテンツを友達と共有すると、サイト上でより多くのトラフィックが生成されます。

1. YouTube ビデオやソーシャルボタンなど、承認されたソーシャルアプリを選択します。

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. 「ソーシャルアプリのアクション」から「**埋め込みコード**」を選択します。

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. サイトのページヘッダー（`<head>`）と本文（`<body>`）のコードをコピーします。

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Web サイトのページヘッダーに、最初のコードスニペットを貼り付けます。

   ![](assets/socialonsite-embedhead.png)

1. ソーシャルアプリを表示したい各ページに、2 番目のコードスニペットを貼り付けます。

   ![](assets/socialonsite-embedwidget.png)

1. ソーシャルアプリのサイズをページ上の特定のディメンションに設定する必要がある場合は、2 番目のコードスニペットに **outerHeight** および **outerWidth** オプションを追加します。例えば、次のように `options='{"outerHeight":400, "outerWidth":600}'` を追加できます。

   ![](assets/socialonsite-resizewidget2.png)

   Marketo ソーシャルアプリによって Web サイトにコンテンツとインタラクティビティが追加され、ファン、訪問者および既存の顧客による自社に関する情報の拡散が促進されます。同時に、プロファイルデータをデータベースに追加して、ソーシャルインフルエンス指標をトラッキングします。

   >[!MORELIKETHIS]
   >
   >* [ソーシャルアプリボタンのカスタマイズ](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [ソーシャル共有要件の設定](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [ランディングページの Facebook への公開](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
