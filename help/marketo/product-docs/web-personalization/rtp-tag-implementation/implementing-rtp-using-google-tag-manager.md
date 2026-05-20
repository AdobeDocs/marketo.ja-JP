---
unique-page-id: 4720145
description: dnl googleを使用したrtpの実装など、Marketo Engageのgoogle tag managerを使用したrtpの実装について説明します。 このガイドを使用して、次のステップを完了してください。
title: Google タグマネージャーを使用した RTP の実装
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
TQID: https://experienceleague.adobe.com/XesXGBf2aDsnsbS2Ro1RLdd1EVrj-mBdCiv8C0dj8NU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 63%

---

# [!DNL Google Tag Manager] を使用した RTP の実装 {#implementing-rtp-using-google-tag-manager}

RTP タグを実装するには、次のインストール手順に従います。

1. [!DNL Google Tag Manager] アカウントにログインします。

1. 新しい&#x200B;**[!UICONTROL タグ]** > **[!UICONTROL タグ設定]** > **[!UICONTROL カスタム HTML タグ ].**&#x200B;を追加します **RTP**&#x200B;と呼んでください。

1. **RTP アカウント**&#x200B;にログインします。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートからJavaScript タグを既に受け取っている場合は、手順6に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. RTP JavaScript タグをコピーし、作成した新しい&#x200B;**カスタム HTML タグ**&#x200B;にペーストします（手順 1）。

1. 「**[!UICONTROL タグをトリガーするルールを追加]**」をクリックします。 「**[!UICONTROL すべてのページ]**」を選択します。

1. 「**[!UICONTROL 保存]**」をクリックして、[新しいバージョンを公開](https://support.google.com/tagmanager/answer/2699097?hl=ja)します。

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   a. これは、web サイトのページで右クリックすることで可能です。 **[!UICONTROL 要素を検査]**&#x200B;に移動して、**RTP** を検索してタグを見つけます。
