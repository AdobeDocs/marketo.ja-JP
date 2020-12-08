---
unique-page-id: 4720149
description: WordpressでのRTPの実装 — Marketto Docs — 製品ドキュメント
title: WordpressでのRTPの実装
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# WordpressでのRTPの実装 {#implementing-rtp-on-wordpress}

RTPタグを実装するには、次のインストール手順に従ってください。

1. WordPressテーマの **header.php** ファイルを開きます ****。

   FTPクライアントを使用してサーバーにアクセスするか、WordPressダッシュボードから直接テーマファイルを編集できます。 ファイルエディターは、サイドバーメニューの「 **外観** 」タブの下にあります。

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. テキストエディターの右側にあるテンプレートファイルのリストで、 **header.phpを探して開きます** 。
1. 「 **アカウント設定」に移動します。**

   サポートからJavaScriptタグを既に受け取っている場合は、手順5に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. 「Domain」で、関連するドメインを探し、「 **Generate Tag**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. RTP JavaScriptタグをコピーして、Webサイトテンプレートに貼り付けます。

   ページのヘッダーにある最初のスクリプト( **`<head> </head>`** タグ間)であることを確認します。

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. header.phpファイルの「 **ファイルを更新** 」をクリックします。
1. すべての `pages including` ランディングページとサブドメインに表示されることを確認します。

   これは、 `website’s` ページを右クリックすると行えます。 「 **表示ページソース」に移動。** タグを見つけるには、 **RTP** を検索します。
