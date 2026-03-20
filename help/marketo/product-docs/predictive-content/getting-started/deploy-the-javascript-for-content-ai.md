---
unique-page-id: 11385053
description: 予測コンテンツ用の RTP Web Personalization タグを生成して配置する方法を説明します。 ページヘッダーにコピーし、カバレッジを確認し、切り替えがオンのままであることを確認します。
title: Content-AI 用の JavaScript のデプロイ
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
source-git-commit: cd7a000c415bedd561aa509e375ba0dee8e81d9f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 82%

---

# Content-AI 用の JavaScript のデプロイ {#deploy-the-javascript-for-content-ai}

予測コンテンツを使用するには、RTP（web パーソナライゼーション）のタグを生成し、設定する必要があります。

## タグの生成 {#generate-tag}

1. 予測コンテンツアカウントにログインします。「**[!UICONTROL アカウント設定]**」に移動します。

   ![](assets/settings-dropdown-account-hands.png)

1. 「**[!UICONTROL ドメイン設定]**」で、関連するドメインを探し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/generate-tag.png)

1. 「Web パーソナライゼーション」タグをコピーして、web サイトの HTML に貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Web パーソナライゼーションの JavaScript タグをコピーし、ページヘッダー（`<head> </head>` タグの間）の最初のスクリプトとして貼り付けます。実装に関する詳細な手順は、[こちら](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)を参照してください。

1. ランディングページとサブドメインも含めてすべてのページにタグがあることを確認します。Web サイトのページを右クリックして、これを確認します。Web ブラウザーで「**[!UICONTROL ページソースを表示]**」に移動します。「RTP」を検索します。

1. タグの切替スイッチが「**[!UICONTROL ON]**」に設定されていることを確認します。
