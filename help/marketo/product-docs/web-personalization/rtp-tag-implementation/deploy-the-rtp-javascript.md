---
unique-page-id: 4719332
description: rtp javascriptのデプロイを含む、Marketo Engageでのrtp javascriptのデプロイについて説明します。 このガイドを使用して、次のステップを完了してください。
title: RTP JavaScript をデプロイする
exl-id: ef96a7f4-3942-4325-bb0f-7647ff2b33b6
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XUylNa8clUib-aMhpAR8fjeu4pHRA8KSQydSH1AVxF8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 88%

---

# RTP JavaScript をデプロイする {#deploy-the-rtp-javascript}

RTP タグを生成して設定するには、以下のインストール手順に従ってください

## [!UICONTROL タグの生成] {#generate-tag}

1. RTP アカウントにログインします。 「**[!UICONTROL アカウント設定]**」に移動します。

   ![](assets/image2014-12-1-23-3a3-3a12.png)

1. 「**[!UICONTROL ドメイン]**」と「**[!UICONTROL ドメイン設定]**」で、関連するドメインを探し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-12-1-23-3a5-3a35.png)

1. 「Web パーソナライゼーション（RTP）」タグをコピーして web サイトにペーストします。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >「RTP JavaScript」タグをコピーし、ページのヘッダー内の最初のスクリプトとして、`<head> </head>` タグの間に貼り付けます。

   ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認してください。 Web サイトのページを右クリックして、これを確認します。 Web ブラウザーで「ページソースを表示」に移動します。 「RTP」を検索します。

1. [!UICONTROL タグ]の切り替え設定を&#x200B;**[!UICONTROL オン]**&#x200B;にします。

   [!UICONTROL タグ]の切り替え設定が「[!UICONTROL オン]」になっていることを確認します。 「組織」タブにデータが入り始めます。

   これで、RTP タグが設定され、[セグメント](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md)とリアルタイムキャンペーンの作成を開始する準備が整いました。

1. タグがすべてのページにあることを確認します。
