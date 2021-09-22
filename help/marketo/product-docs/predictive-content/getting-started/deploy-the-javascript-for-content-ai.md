---
unique-page-id: 11385053
description: Content-AI 用の JavaScript のデプロイ - Marketo ドキュメント - 製品ドキュメント
title: Content-AI 用の JavaScript のデプロイ
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '139'
ht-degree: 100%

---

# Content-AI 用の JavaScript のデプロイ {#deploy-the-javascript-for-content-ai}

予測コンテンツを使用するには、RTP（web パーソナル）のタグを生成し、設定する必要があります。

## タグの生成 {#generate-tag}

1. 予測コンテンツアカウントにログインします。「**アカウント設定**」に移動します。

   ![](assets/settings-dropdown-account-hands.png)

1. 「**ドメイン設定**」で、関連するドメインを探し、「**タグを生成**」をクリックします。

   ![](assets/generate-tag.png)

1. 「Web パーソナライゼーション」タグをコピーして、web サイトの HTML に貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Web パーソナライズの JavaScript タグをコピーし、ページヘッダー（`<head> </head>` タグの間）の最初のスクリプトとして貼り付けます。実装に関する詳細な手順は、[こちら](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)を参照してください。

1. ランディングページとサブドメインも含めてすべてのページにタグがあることを確認します。Web サイトのページを右クリックして、これを確認します。Web ブラウザーで「**ページソースを表示**」に移動します。「RTP」を検索します。

1. タグの切り替えが「**ON**」に設定されていることを確認します。
