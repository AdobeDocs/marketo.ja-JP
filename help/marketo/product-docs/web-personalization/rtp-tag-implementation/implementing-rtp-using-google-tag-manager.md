---
unique-page-id: 4720145
description: Google タグマネージャーを使用した RTP の実装 - Marketo ドキュメント - 製品ドキュメント
title: Google タグマネージャーを使用した RTP の実装
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 100%

---

# [!DNL Google Tag Manager] を使用した RTP の実装 {#implementing-rtp-using-google-tag-manager}

RTP タグを実装するには、次のインストール手順に従います。

1. [!DNL Google Tag Manager] アカウントにログインします。

1. 新しい&#x200B;**[!UICONTROL タグ]**／**[!UICONTROL タグ設定]**／**[!UICONTROL カスタム HTML タグ]を追加します。**「**RTP**」と名前を付けます。

1. **RTP アカウント**&#x200B;にログインします。

1. 「**[!UICONTROL アカウント設定]**」に移動します。

   サポートから既に JavaScript タグを受け取っている場合は、手順 6 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. [!UICONTROL ドメイン]で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. RTP JavaScript タグをコピーし、作成した新しい&#x200B;**カスタム HTML タグ**&#x200B;にペーストします（手順 1）。

1. 「**[!UICONTROL タグをトリガーするルールを追加]**」をクリックします。「**[!UICONTROL すべてのページ]**」を選択します。

1. 「**[!UICONTROL 保存]**」をクリックして、[新しいバージョンを公開](https://support.google.com/tagmanager/answer/2699097?hl=ja)します。

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   a. これは、Web サイトのページを右クリックすることでおこなえます。**[!UICONTROL 要素を検査]**&#x200B;に移動して、**RTP** を検索してタグを見つけます。
