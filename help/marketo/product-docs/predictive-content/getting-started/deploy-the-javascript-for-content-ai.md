---
unique-page-id: 11385053
description: JavaScriptのコンテンツAI向けデプロイ — Marketto Docs — 製品ドキュメント
title: JavaScriptのコンテンツ用の導入 —AI
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# JavaScriptのコンテンツ用の導入 —AI {#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>購入日に応じて、マーケティング担当購読に「予測コンテンツ」または「コンテンツ`<sup>AI</sup>`」が含まれる場合があります。 予測コンテンツを使用するユーザーの場合、Marketing Cloudでは、2018年4月31日までコンテンツ`<sup>AI</sup>` 分析機能を有効にしています。 これらの機能をこの日以降に引き続きご利用いただくには、マーケティング担当者カスタマーサクセスマネージャーにお問い合わせの上、マーケティングコンテンツにアップグレードしてください`<sup>AI</sup>`。

予測コンテンツを使用するには、RTP（Webパーソナライゼーション）を生成し、設定する必要があります `tag.`

## タグの生成 {#generate-tag}

1. 予測コンテンツアカウントにログインします。 「 **アカウント設定**」に移動します。

   ![](assets/settings-dropdown-account-hands.png)

1. 「 **Domain Configuration**」で、関連するドメインを探し、「 **Generate Tag」をクリックします。**

   ![](assets/generate-tag.png)

1. Webパーソナライゼーションタグをコピーして、WebサイトのHTMLに貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >ウェブパーソナライゼーションのJavaScriptタグをコピーし、ページのヘッダーの最初のスクリプトとして、タグ間に貼り付け `<head> </head>` ます。 詳しい [導入手順については、こちらを参照してください](http://docs.marketo.com/display/docs/rtp+tag+implementation)[。](http://pages2.marketo.com/rtp-implementation.html)

1. タグがランディングページやサブドメインを含むすべてのページに表示されることを確認します。 ページを右クリックして、これを確認してくだ `website’s` さい。 Webブラウザーで「 **表示ページソース** 」に移動します。 検索：「RTP」
1. 「タグ」トグルが「オン」に設定されていることを確認 **します**。

