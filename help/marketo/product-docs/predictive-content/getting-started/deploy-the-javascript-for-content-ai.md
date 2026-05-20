---
unique-page-id: 11385053
description: 予測コンテンツ用のRTP Web Personalization タグを生成して配置する方法について説明します。 それをページヘッドにコピーし、カバー範囲を確認し、トグルがオンのままであることを確認します。
title: Content-AI 用の JavaScript のデプロイ
exl-id: d48bfd1b-73e8-4013-88d6-8750e4ef532b
feature: Predictive Content
TQID: https://experienceleague.adobe.com/LHzl0KuIoJvZ99eFWGFE6RdDW1xRxBS4LG3XU9ujj4U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 82%

---

# Content-AI 用の JavaScript のデプロイ {#deploy-the-javascript-for-content-ai}

予測コンテンツを使用するには、RTP（web パーソナライゼーション）のタグを生成し、設定する必要があります。

## タグの生成 {#generate-tag}

1. 予測コンテンツアカウントにログインします。 「**[!UICONTROL アカウント設定]**」に移動します。

   ![](assets/settings-dropdown-account-hands.png)

1. 「**[!UICONTROL ドメイン設定]**」で、関連するドメインを探し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/generate-tag.png)

1. 「Web パーソナライゼーション」タグをコピーして、web サイトの HTML に貼り付けます。

   ![](assets/web-personalization-tag.png)

   >[!NOTE]
   >
   >Web パーソナライゼーションの JavaScript タグをコピーし、ページヘッダー（`<head> </head>` タグの間）の最初のスクリプトとして貼り付けます。 実装に関する詳細な手順は、[こちら](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md)を参照してください。

1. ランディングページとサブドメインも含めてすべてのページにタグがあることを確認します。 Web サイトのページを右クリックして、これを確認します。 Web ブラウザーで「**[!UICONTROL ページソースを表示]**」に移動します。 「RTP」を検索します。

1. タグの切替スイッチが「**[!UICONTROL ON]**」に設定されていることを確認します。
