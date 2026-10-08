---
unique-page-id: 4720149
description: dnl wordpressでのrtpの実装など、Marketo Engageでのwordpressでのrtpの実装について説明します。 このガイドを使用して、次のステップを完了してください。
title: Wordpress での RTP の実装​
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/5V3CEgasEJi4zrYoezh8Tt340VGHNNHaliF2wdbBLwY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '202'
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

1. [!UICONTROL ドメイン]で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. RTP JavaScript タグをコピーして、Web サイトテンプレートにペーストします。

   a. ページのヘッダー（**`<head> </head>`** タグ間）にある最初のスクリプトであることを確認してください。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. header.php ファイルの&#x200B;**[!UICONTROL ファイルの更新]**&#x200B;をクリックします。

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   a. これは、web サイトのページを右クリックすることでおこなえます。 **[!UICONTROL ページを表示Source]に移動します。** タグを見つけるために&#x200B;**RTP**&#x200B;を検索します。
