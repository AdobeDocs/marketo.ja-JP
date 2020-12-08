---
unique-page-id: 4720145
description: Google Tag Managerを使用したRTPの実装 — Marketto Docs — 製品ドキュメント
title: Google Tag Managerを使用したRTPの実装
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 0%

---


# Google Tag Managerを使用したRTPの実装 {#implementing-rtp-using-google-tag-manager}

RTPを実装するには、次のインストール手順 `tag please` に従います。

1. Google Tag Managerアカウントにログインします。

1. 新追加しいタグ/タグ設定/カスタムHTMLタグ**** **RTPと呼びます**。

1. RTPアカウントにログインします**。**

1. 「**アカウント設定」に移動します。**

   1. サポートからJavaScriptタグを既に受け取っている場合は、手順6に進みます。

      ![](assets/image2014-11-30-15-3a19-3a21.png)

1. 「Domain」で、関連するドメインを探し、「 **Generate Tag**」をクリックします。

   ** ![](assets/image2014-11-30-15-3a20-3a17.png)

   **

1. RTP JavaScriptタグをコピーし、作成した新しい **カスタムHTMLタグに貼り付けます** （手順1）。

1. タグを実行するには、 **+追加ルールをクリックします**。 「 **すべてのページ**」を選択します。

1. 「**保存**」をクリックし、新しいバージョンを [発行します](https://support.google.com/tagmanager/answer/2699097?hl=en)。

1. すべての `pages, including` ランディングページとサブドメインに表示されることを確認します。

   1. これは、 `website’s` ページを右クリックすると行えます。 「**Inspect要素」に移動します。 ****RTP **を検索してタグを探します。

