---
unique-page-id: 4720215
description: Wordpress Enterprise での RTP の実装 - Marketo ドキュメント - 製品ドキュメント
title: Wordpress Enterprise での RTP の実装
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '106'
ht-degree: 100%

---

# Wordpress での RTP の実装エンタープライズ {#implementing-rtp-on-wordpress-enterprise}

RTP タグを実装するには、次のインストール手順に従います。

1. 「**アカウント設定**」に移動します。

   a サポートから既に JavaScript タグを受け取っている場合は、手順 3 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. ドメインで、該当するドメインを選択し、「**タグの生成**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. RTP JavaScript タグをコピーします。

1. WordPress アカウントに管理者ユーザーとしてログインします。

   a. **表示方法**&#x200B;の下にある「**カスタム JavaScript**」に移動します。b. RTP JavaScript タグを既存のコードの直後にペーストします。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >コードをペーストすると、次のタグが除外されます。
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >スクリプト自体のみを挿入します。

1. 「**更新**」をクリックします。
