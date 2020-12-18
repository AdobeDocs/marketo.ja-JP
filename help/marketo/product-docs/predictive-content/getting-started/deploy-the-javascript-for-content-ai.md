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


# JavaScript for Content-AIの導入{#deploy-the-javascript-for-content-ai}

>[!NOTE]
>
>購入日に応じて、マーケティング担当者の購読に、マーケティング担当者の予測コンテンツまたはコンテンツ`<sup>AI</sup>`が含まれる場合があります。 予測コンテンツを使用するユーザーの場合、Marketing Cloudでは、2018年4月30日までコンテンツ`<sup>AI</sup>`分析機能を有効にしています。 これらの機能をこの日以降に引き続き使用するには、マーケティング担当カスタマーサクセスマネージャーにお問い合わせの上、マーケティングコンテンツ`<sup>AI</sup>`にアップグレードしてください。

予測コンテンツを使用するには、RTP（Webパーソナライゼーション） `tag.`を生成して設定する必要があります

## タグを生成{#generate-tag}

1. 予測コンテンツアカウントにログインします。 「**アカウント設定**」に移動します。

   ![](assets/settings-dropdown-account-hands.png)

1. **ドメイン設定**&#x200B;で、関連するドメインを探し、**タグの生成をクリックします。**

   ![](assets/generate-tag.png)

1. Webパーソナライゼーションタグをコピーして、WebサイトのHTMLに貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >ウェブパーソナライゼーションのJavaScriptタグをコピーし、ページのヘッダーの`<head> </head>`タグの間に最初のスクリプトとして貼り付けます。 [実装の手順の詳細については、](http://docs.marketo.com/display/docs/rtp+tag+implementation) [を参照してください。](http://pages2.marketo.com/rtp-implementation.html)

1. タグがランディングページやサブドメインを含むすべてのページに表示されることを確認します。 `website’s`ページを右クリックして、これを確認します。 Webブラウザーで&#x200B;**表示ページソース**&#x200B;に移動します。 検索：「RTP」
1. タグの切り替えが&#x200B;**ON**&#x200B;に設定されていることを確認します。

