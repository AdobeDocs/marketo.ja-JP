---
unique-page-id: 4720149
description: dnl wordpressでのrtpの実装など、Marketo Engageでのwordpressでのrtpの実装について説明します。 このガイドを使用して、次のステップを完了してください。
title: Wordpress での RTP の実装
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 66%

---

# [!DNL Wordpress] での RTP の実装 {#implementing-rtp-on-wordpress}

[!UICONTROL RTP タグ]を実装するには、次のインストール手順に従います。

1. **[!DNL WordPress]テーマ**&#x200B;の **header.php** ファイルを開きます。

   FTP クライアントを使用してサーバーにアクセスするか、[!DNL WordPress] のダッシュボードから直接テーマファイルを編集できます。 ファイルエディターは、サイドバーメニューの「**[!UICONTROL 外観]**」タブにあります。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. テキストエディターの右側にあるテンプレートファイルのリストで、**header.php** を探して開きます。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートからJavaScript タグを既に受け取っている場合は、手順5に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. RTP JavaScript タグをコピーして、Web サイトテンプレートにペーストします。

   a. ページのヘッダー（**`<head> </head>`** タグ間）にある最初のスクリプトであることを確認してください。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. header.php ファイルの&#x200B;**[!UICONTROL ファイルの更新]**&#x200B;をクリックします。

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   a. これは、web サイトのページを右クリックすることでおこなえます。 **[!UICONTROL ページを表示Source]に移動します。** タグを見つけるために&#x200B;**RTP**&#x200B;を検索します。
