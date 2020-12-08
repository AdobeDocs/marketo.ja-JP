---
unique-page-id: 4719332
description: RTP JavaScript - Marketto Docs — 製品ドキュメントの導入
title: RTP JavaScriptのデプロイ
translation-type: tm+mt
source-git-commit: c8a77dc84c023e05fbb442f575269aac108ffb29
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# RTP JavaScriptのデプロイ {#deploy-the-rtp-javascript}

RTPタグを生成し、設定するには、次のインストール手順に従ってください

## タグの生成 {#generate-tag}

1. RTPアカウントにログインします。 「 **アカウント設定**」に移動します。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 「 **Domain** and **Domain Configuration**」で、関連するドメインを探し、「 **Generate Tag」をクリックします。**

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. Webパーソナライゼーション(RTP)タグをコピーしてWebサイトに貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >RTP JavaScriptタグをコピーし、ページのヘッダー内の最初のスクリプトとして、タグ間に貼り付け `<head> </head>` ます。

   タグがランディングページやサブドメインを含むすべてのページに表示されることを確認します。 Webサイトのページを右クリックして、これを確認します。 Webブラウザーで「表示ページソース」に移動します。 検索：「RTP」

1. タグの切り替えを **オンに設定**。

   「タグ」トグルが「オン」に設定されていることを確認します。 「組織」タブにデータフローが表示されていることを開始に確認する必要があります。

   これで、RTPタグが設定され、セグメントとリアルタイムキャンペーンの [作成を開始できる状態になりました](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) 。

1. タグがすべてのページにあることを確認します。

>[!MORELIKETHIS]
>
>* [RTPタグの実装](http://docs.marketo.com/display/docs/rtp+tag+implementation)

