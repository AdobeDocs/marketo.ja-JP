---
unique-page-id: 4720149
description: Wordpress での RTP の実装 — Marketo ドキュメント — 製品ドキュメント
title: Wordpress での RTP の実装
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 100%

---

# [!DNL Wordpress] での RTP の実装 {#implementing-rtp-on-wordpress}

[!UICONTROL RTP タグ]を実装するには、次のインストール手順に従います。

1. **[!DNL WordPress]テーマ**&#x200B;の **header.php** ファイルを開きます。

   FTP クライアントを使用してサーバーにアクセスするか、[!DNL WordPress] のダッシュボードから直接テーマファイルを編集できます。ファイルエディターは、サイドバーメニューの「**[!UICONTROL 外観]**」タブにあります。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. テキストエディターの右側にあるテンプレートファイルのリストで、**header.php** を探して開きます。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートから既に JavaScript タグを受け取っている場合は、手順 5 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. [!UICONTROL ドメイン]で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. RTP JavaScript タグをコピーして、Web サイトテンプレートにペーストします。

   a. ページのヘッダーで必ず最初のスクリプトになる位置に貼り付けてください。つまり、**`<head> </head>`** タグの間です。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. header.php ファイルの&#x200B;**[!UICONTROL ファイルの更新]**&#x200B;をクリックします。

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   a. これは、Web サイトのページを右クリックすることでおこなえます。「**[!UICONTROL ページソースを表示]」に移動します。****RTP** を検索してタグを見つけます。
