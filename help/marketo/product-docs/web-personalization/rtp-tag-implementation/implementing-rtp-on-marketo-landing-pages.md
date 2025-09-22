---
unique-page-id: 4720151
description: Marketo ランディングページでの RTP の実装 - Marketo ドキュメント - 製品ドキュメント
title: Marketo ランディングページでの RTP の実装
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 100%

---

# Marketo ランディングページでの RTP の実装 {#implementing-rtp-on-marketo-landing-pages}

[!UICONTROL RTP タグ]を実装するには、次のインストール手順に従います。

1. **[!UICONTROL デザインスタジオ]に移動します。** 編集する項目を開きます。**[!UICONTROL テンプレートのアクション]**／**[!UICONTROL 下書きの編集]**&#x200B;を選択します。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 「**HTML ソース**」タブでテンプレートを変更します。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. RTP アカウントで、「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートから既に JavaScript タグを受け取っている場合は、手順 5 に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを見つけ、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. RTP JavaScript タグをコピーし、すべてのランディングページテンプレートに **`<head> </head>`** タグの間でペーストします。

1. 「**[!UICONTROL 保存]**」をクリックして、ウィンドウを&#x200B;**[!UICONTROL 閉じます]**。

1. **[!UICONTROL Design Studio]** で、**[!UICONTROL テンプレートのアクション]**&#x200B;からランディングページを承認して、「**[!UICONTROL 承認]**」をクリックします。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後に、テンプレートの変更を有効にするには、そのテンプレートを使用してランディングページを&#x200B;**再承認**&#x200B;する必要があります。メインの「[!UICONTROL ランディングページ]」セクションから、一度にすべてのランディングページを再承認できます。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   これは、web サイトのページを右クリックすることでおこなえます。「**[!UICONTROL ページソースを表示]」に移動します。****[!UICONTROL RTP]** を検索してタグを見つけます。
