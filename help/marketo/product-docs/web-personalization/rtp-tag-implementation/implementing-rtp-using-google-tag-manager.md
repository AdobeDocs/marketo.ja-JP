---
unique-page-id: 4720145
description: Google Tag Managerを使用したRTPの実装 — Marketto Docs — 製品ドキュメント
title: Google Tag Managerを使用したRTPの実装
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# Google Tag Manager {#implementing-rtp-using-google-tag-manager}を使用したRTPの実装

RTPタグを実装するには、次のインストール手順に従ってください。

1. Google Tag Managerアカウントにログインします。

1. 新追加しいタグ/タグ設定/カスタムHTMLタグ******RTP**&#x200B;と呼びます。

1. RTPアカウントにログインします**。**

1. 「**アカウント設定**」に移動します。

   a.サポートからJavaScriptタグを既に受け取っている場合は、手順6に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. RTP JavaScriptタグをコピーして、作成した新しい&#x200B;**カスタムHTMLタグ**&#x200B;に貼り付けます（手順1）。

1. **+追加 Rule to Fire Tag**&#x200B;をクリックします。 「**すべてのページ**」を選択します。

1. 「**保存**」をクリックし、[新しいバージョン](https://support.google.com/tagmanager/answer/2699097?hl=en)を公開します。

1. ランディングページやサブドメインを含むすべてのページに表示されることを確認します。

   a.これは、Webサイトのページを右クリックすると行えます。 **Inspect要素**&#x200B;に移動し、**RTP**&#x200B;を探してタグを探します。
