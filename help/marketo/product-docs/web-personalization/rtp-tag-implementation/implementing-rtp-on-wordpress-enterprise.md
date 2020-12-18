---
unique-page-id: 4720215
description: Wordpress EnterpriseでのRTPの実装 — Marketto Docs — 製品ドキュメント
title: Wordpress EnterpriseでのRTPの実装
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Wordpress EnterpriseでのRTPの実装{#implementing-rtp-on-wordpress-enterprise}

RTPタグを実装するには、次のインストール手順に従ってください。

1. 「**アカウント設定」に移動します。**

   1. サポートからJavaScriptタグを既に受け取っている場合は、手順3に進みます。\
      ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. RTP JavaScriptタグをコピーします。
1. WordPressアカウントに管理者ユーザーとしてログインします

   1. 「**外観**」の下の「**カスタムJavaScript**」に移動します。
   1. RTP Javascriptタグを既存のコードの直後に貼り付けます。

      ![](assets/image2014-12-3-17-3a51-3a46.png)
   >[!CAUTION]
   >
   >コードを貼り付けると、次のタグが除外されます。
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >    
   >スクリプト自体をONLYで挿入します。

1. 「**更新**」をクリックします。
