---
unique-page-id: 4720215
description: Wordpress EnterpriseでのRTPの実装 —Marketoドキュメント — 製品ドキュメント
title: Wordpress EnterpriseでのRTPの実装
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Wordpress EnterpriseでのRTPの実装{#implementing-rtp-on-wordpress-enterprise}

RTPタグを実装するには、次のインストール手順に従ってください。

1. 「**アカウント設定**」に移動します。

   a.サポートからJavaScriptタグを既に受け取っている場合は、手順3に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 「Domain」で、関連するドメインを探し、「**Generate Tag**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. RTP JavaScriptタグをコピーします。

1. WordPressアカウントに管理者ユーザーとしてログインします

   a.「**外観**」の下の「**カスタムJavaScript**」に移動します。
b.RTP Javascriptタグを既存のコードの直後に貼り付けます。

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
