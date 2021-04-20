---
unique-page-id: 11385053
description: JavaScriptのコンテンツ用のデプロイ — AI -Marketoドキュメント — 製品ドキュメント
title: JavaScriptのコンテンツ用の導入 —AI
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 1%

---

# JavaScript for Content-AIの導入{#deploy-the-javascript-for-content-ai}

予測コンテンツを使用するには、RTP(Web Personalization)タグを生成し、設定する必要があります。

## タグの生成 {#generate-tag}

1. 予測コンテンツアカウントにログインします。 「**アカウント設定**」に移動します。

   ![](assets/settings-dropdown-account-hands.png)

1. **ドメイン設定**&#x200B;で、関連するドメインを探し、**タグを生成**&#x200B;をクリックします。

   ![](assets/generate-tag.png)

1. Webパーソナライゼーションタグをコピーして、WebサイトのHTMLに貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >ウェブパーソナライゼーションのJavaScriptタグをコピーし、ページのヘッダーの`<head> </head>`タグの間に最初のスクリプトとして貼り付けます。 [導入手順の詳細については、](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)を参照してください。

1. タグがランディングページやサブドメインを含むすべてのページに表示されることを確認します。 Webサイトのページを右クリックして、これを確認します。 Webブラウザーで&#x200B;**表示ページソース**&#x200B;に移動します。 検索：「RTP」

1. タグの切り替えが&#x200B;**ON**&#x200B;に設定されていることを確認します。
