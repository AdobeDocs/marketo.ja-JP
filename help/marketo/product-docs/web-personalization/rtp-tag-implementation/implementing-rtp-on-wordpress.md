---
unique-page-id: 4720149
description: Wordpress での RTP の実装 — Marketo ドキュメント — 製品ドキュメント
title: Wordpress での RTP の実装
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 69%

---

# [!DNL Wordpress] への RTP の実装 {#implementing-rtp-on-wordpress}

[!UICONTROL RTP タグを実装するには &#x200B;] 以下のインストール手順に従ってください。

1. **テーマの** header.php **[!DNL WordPress]ファイルを開き** す。

   FTP クライアントを使用してサーバーにアクセスしたり、[!DNL WordPress] ダッシュボードから直接テーマファイルを編集したりできます。 ファイルエディターは、サイドバーメニューの「**[!UICONTROL 外観]**」タブにあります。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. テキストエディターの右側にあるテンプレートファイルのリストで、**header.php** を探して開きます。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a サポートから既に JavaScript タグを受け取っている場合は、手順 5 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. [!UICONTROL &#x200B; ドメイン &#x200B;] の下で関連するドメインを見つけて、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. RTP JavaScript タグをコピーして、Web サイトテンプレートにペーストします。

   a. ページのヘッダーで必ず最初のスクリプトになる位置に貼り付けてください。つまり、**`<head> </head>`** タグの間です。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. header.php ファイルの&#x200B;**[!UICONTROL ファイルの更新]**&#x200B;をクリックします。

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   a. これは、Web サイトのページを右クリックすることでおこなえます。**[!UICONTROL ページを表示Source] に移動します。**」に移動します。**RTP** を検索してタグを見つけます。
