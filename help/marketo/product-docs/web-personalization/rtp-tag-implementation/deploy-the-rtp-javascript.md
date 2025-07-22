---
unique-page-id: 4719332
description: RTP JavaScript をデプロイする — Marketo ドキュメント — 製品ドキュメント
title: RTP JavaScript をデプロイする
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 90%

---

# RTP JavaScript をデプロイする {#deploy-the-rtp-javascript}

RTP タグを生成して設定するには、以下のインストール手順に従ってください

## [!UICONTROL  タグを生成 ] {#generate-tag}

1. RTP アカウントにログインします。「**[!UICONTROL アカウント設定]**」に移動します。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 「**[!UICONTROL ドメイン]**」と「**[!UICONTROL ドメイン設定]**」で、関連するドメインを探し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 「ウェブパーソナライズ（RTP）」タグをコピーしてウェブサイトにペーストします。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >「RTP JavaScript」タグをコピーし、ページのヘッダー内の最初のスクリプトとして、`<head> </head>` タグの間に貼り付けます。

   ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認してください。Web サイトのページを右クリックして、これを確認します。Web ブラウザーで「ページソースを表示」に移動します。「RTP」を検索します。

1. [!UICONTROL  タグ ] 切り替えを **[!UICONTROL オン]** に設定。

   [!UICONTROL  タグ ] 切り替えが [!UICONTROL  オン ] に設定されていることを確認します。 「組織」タブにデータが入り始めます。

   これで、RTP タグが設定され、[セグメント](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)とリアルタイムキャンペーンの作成を開始する準備が整いました。

1. タグがすべてのページにあることを確認します。
