---
unique-page-id: 11385053
description: JavaScriptのコンテンツAI向けデプロイ — Marketto Docs — 製品ドキュメント
title: JavaScriptのコンテンツ用の導入 —AI
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---


# JavaScript for Content-AIの導入{#deploy-the-javascript-for-content-ai}

予測コンテンツを使用するには、RTP(Web Personalization)タグを生成し、設定する必要があります。

## タグを生成{#generate-tag}

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
