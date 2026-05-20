---
unique-page-id: 4720151
description: Adobe Marketo Engageへのrtpの実装など、Marketo Engageのランディングページにrtpを実装する方法について解説します。 このガイドを使用して、次のステップを完了してください。
title: Marketo ランディングページでの RTP の実装
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
TQID: https://experienceleague.adobe.com/scyZfbFBloPu8JRfJiMjm62AFCHM7WCxaats3qssq2A
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 213
ht-degree: 70%

---

# Marketo ランディングページでの RTP の実装 {#implementing-rtp-on-marketo-landing-pages}

[!UICONTROL RTP タグ]を実装するには、次のインストール手順に従います。

1. **[!UICONTROL デザインスタジオ ]に移動します。** 編集する項目を開きます。 **[!UICONTROL テンプレートのアクション]**／**[!UICONTROL 下書きの編集]**&#x200B;を選択します。

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. 「**HTML ソース**」タブでテンプレートを変更します。

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. RTP アカウントで、「**[!UICONTROL アカウント設定]**」に移動します。

   a. サポートからJavaScript タグを既に受け取っている場合は、手順5に進みます。

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. 「[!UICONTROL ドメイン]」で、該当するドメインを選択し、「**[!UICONTROL タグを生成]**」をクリックします。

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. RTP JavaScript タグをコピーし、すべてのランディングページテンプレートに **`<head> </head>`** タグの間でペーストします。

1. 「**[!UICONTROL 保存]**」をクリックして、ウィンドウを&#x200B;**[!UICONTROL 閉じます]**。

1. **[!UICONTROL Design Studio]** で、**[!UICONTROL テンプレートのアクション]**&#x200B;からランディングページを承認して、「**[!UICONTROL 承認]**」をクリックします。

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. 最後に、テンプレートの変更を有効にするには、そのテンプレートを使用してランディングページを&#x200B;**再承認**&#x200B;する必要があります。 メインの「[!UICONTROL ランディングページ]」セクションから、一度にすべてのランディングページを再承認できます。

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. ランディングページとサブドメインも含めて、すべてのページにタグがあることを確認します。

   これは、web サイトのページを右クリックすることでおこなえます。 **[!UICONTROL ページを表示Source]に移動します。** タグを見つけるために&#x200B;**[!UICONTROL RTP]**&#x200B;を検索します。
