---
unique-page-id: 4720215
description: wordpressでのrtpの実装など、Marketo Engageでのwordpress enterpriseでのrtpの実装について説明します。 このガイドを使用して、次のステップを完了してください。
title: Wordpress Enterprise での RTP の実装
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/S0LvRrD1V6hkWN5L5TlnoaIqcDvXLjfm5do2-1WQTNw'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
    internal-label: Implementation
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 57%
---
# Wordpress Enterprise での RTP の実装 {#implementing-rtp-on-wordpress-enterprise}

[!UICONTROL RTP タグ]を実装するには、次のインストール手順に従います。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートからJavaScript タグを既に受け取っている場合は、手順3に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. RTP JavaScript タグをコピーします。

1. [!DNL WordPress] アカウントに管理者ユーザとしてログインします。

   a. **[!UICONTROL アピアランス]**&#x200B;で、**[!UICONTROL カスタム JavaScript]**&#x200B;に移動します。
   b. 既存のコードの直後にRTP Javascript タグを貼り付けます。

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >コードをペーストする際は、次のタグを除外してください。
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >スクリプト自体のみを挿入します。

1. 「**[!UICONTROL 更新]**」をクリックします。
