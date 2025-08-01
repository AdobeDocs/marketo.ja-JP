---
unique-page-id: 4720151
description: Marketo ランディングページでの RTP の実装 - Marketo ドキュメント - 製品ドキュメント
title: Marketo ランディングページでの RTP の実装
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 80%

---

# Marketo ランディングページでの RTP の実装 {#implementing-rtp-on-marketo-landing-pages}

[!UICONTROL RTP タグを実装するには &#x200B;] 以下のインストール手順に従ってください。

1. **[!UICONTROL Design Studio] に移動します。** 編集する項目を開きます。**[!UICONTROL テンプレートのアクション]**／**[!UICONTROL 下書きの編集]**&#x200B;を選択します。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 「**HTML ソース**」タブでテンプレートを変更します。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. RTP アカウントで、「**[!UICONTROL アカウント設定]**」に移動します。

   a サポートから既に JavaScript タグを受け取っている場合は、手順 5 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. [!UICONTROL &#x200B; ドメイン &#x200B;] の下で関連するドメインを見つけて、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. RTP JavaScript タグをコピーし、すべてのランディングページテンプレートに **`<head> </head>`** タグの間でペーストします。

1. 「**[!UICONTROL 保存]**」をクリックして、ウィンドウを&#x200B;**[!UICONTROL 閉じます]**。

1. **[!UICONTROL Design Studio]** で、**[!UICONTROL テンプレートのアクション]**&#x200B;からランディングページを承認して、「**[!UICONTROL 承認]**」をクリックします。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後に、テンプレートの変更を有効にするには、そのテンプレートを使用してランディングページを&#x200B;**再承認**&#x200B;する必要があります。メインの [!UICONTROL &#x200B; ランディングページ &#x200B;] セクションから、すべてを一度に再承認できます。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   これは、web サイトのページを右クリックすることでおこなえます。**[!UICONTROL ページを表示Source] に移動します。**」に移動します。**[!UICONTROL RTP]** を検索してタグを見つけます。
