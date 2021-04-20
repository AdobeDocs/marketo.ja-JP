---
unique-page-id: 4720149
description: WordpressでのRTPの実装 —Marketoドキュメント — 製品ドキュメント
title: WordpressでのRTPの実装
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# WordpressでのRTPの実装{#implementing-rtp-on-wordpress}

RTPタグを実装するには、次のインストール手順に従ってください。

1. **WordPressテーマ**&#x200B;の&#x200B;**header.php**&#x200B;ファイルを開きます。

   FTPクライアントを使用してサーバーにアクセスするか、WordPressダッシュボードから直接テーマファイルを編集できます。 ファイルエディターは、サイドバーメニューの「**外観**」タブの下にあります。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. テキストエディターの右側にあるテンプレートファイルのリストで、**header.php**&#x200B;を探して開きます。

1. 「**アカウント設定**」に移動します。

   a.サポートからJavaScriptタグを既に受け取っている場合は、手順5に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. RTP JavaScriptタグをコピーして、Webサイトテンプレートに貼り付けます。

   a.ページのヘッダー（**`<head> </head>`**&#x200B;タグの間）の最初のスクリプトであることを確認します。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. header.phpファイルの&#x200B;**更新ファイル**&#x200B;をクリックします。

1. ランディングページとサブドメインを含むすべてのページに表示されることを確認します。

   a.これは、ウェブサイトのページを右クリックすると行えます。 **表示ページソースに移動します。** RTPを検索して、タグを探し **** ます。
