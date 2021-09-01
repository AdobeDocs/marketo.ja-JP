---
unique-page-id: 4719332
description: RTP JavaScript をデプロイする — Marketo ドキュメント — 製品ドキュメント
title: RTP JavaScript をデプロイする
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
source-git-commit: ''
workflow-type: ht
source-wordcount: '167'
ht-degree: 100%

---

# RTP JavaScript をデプロイする {#deploy-the-rtp-javascript}

RTP タグを生成して設定するには、以下のインストール手順に従ってください

## タグの生成 {#generate-tag}

1. RTP アカウントにログインします。「**アカウント設定**」に移動します。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 「**ドメイン**」と「**ドメイン設定**」で、関連するドメインを探し、「**タグを生成**」をクリックします。

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 「Web パーソナライゼーション（RTP）」タグをコピーして Web サイトにペーストします。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >「RTP JavaScript」タグをコピーし、ページのヘッダー内の最初のスクリプトとして、`<head> </head>` タグの間に貼り付けます。

   ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認してください。Web サイトのページを右クリックして、これを確認します。Web ブラウザーで「ページソースを表示」に移動します。「RTP」を検索します。

1. タグの切り替え設定を&#x200B;**オン**&#x200B;にします。

   タグの切り替え設定が「オン」になっていることを確認してください。「組織」タブにデータが入り始めます。

   これで、RTP タグが設定され、[セグメント](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)とリアルタイムキャンペーンの作成を開始する準備が整いました。

1. タグがすべてのページにあることを確認します。
