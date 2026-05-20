---
unique-page-id: 9438139
description: 人をブロックリストに追加する方法を説明します。 特定の人物やドメインにメールが送信されるのを防ぎます。
title: リードをブロックリストに追加
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
TQID: https://experienceleague.adobe.com/wB-xUIHId0Hio0JwB1-yQK-nv52I3oH6NbvZX2FTZ6s
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 195
ht-degree: 39%

---

# リードをブロックリストに追加 {#add-person-to-blocklist}

リードをブロックリストに追加すると、コンテンツを気に入ってくれた有望な人だけにコンテンツを読んでもらえるようになります。

1. 新しい[&#x200B; デフォルトプログラム &#x200B;](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md){target="_blank"}を作成し、「Add to ブロックリスト」という名前を付けます。

1. 「**[!UICONTROL 新規作成]**」をクリックして、「**[!UICONTROL 新規ローカルアセット]**」を選択します。

   ![](assets/add-person-to-blocklist-1.png)

1. 「**[!UICONTROL スマートリスト]**」を選択します。

   ![](assets/add-person-to-blocklist-2.png)

1. リストに名前を付け、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-person-to-blocklist-3.png)

1. スマートブロックリストに追加するスマートリストにすべての人物を追加します。

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >ブロックリストに加えられたリードには、オペレーショナルメールが送信されません。

1. プログラムに戻ります。

   ![](assets/add-person-to-blocklist-5.png)

1. 「**[!UICONTROL 新規作成]**」をクリックして、「**[!UICONTROL 新規スマートキャンペーン]**」を選択します。

   ![](assets/add-person-to-blocklist-6.png)

1. 新しいスマートキャンペーンに名前を付けます。 「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/add-person-to-blocklist-7.png)

1. 「**[!UICONTROL スマートリストのメンバー]**」をドラッグ＆ドロップします。

   ![](assets/add-person-to-blocklist-8.png)

1. 作成したスマートリストを選択します。

   ![](assets/add-person-to-blocklist-9.png)

1. 「**[!UICONTROL フロー]**」タブをクリックします。 「**[!UICONTROL データ値を変更]**」フローアクションをドラッグ&amp;ドロップします。

   ![](assets/add-person-to-blocklist-10.png)

1. **[!UICONTROL 属性]** ドロップダウンで、「**[!UICONTROL リストされているブロック]**」を選択し、**[!UICONTROL 新しい値]**&#x200B;を&#x200B;**[!UICONTROL true]**&#x200B;に設定します。

   ![](assets/add-person-to-blocklist-11.png)

1. 「**[!UICONTROL スケジュール]**」タブをクリックし、**[!UICONTROL 1回実行]**&#x200B;を選択します。

   ![](assets/add-person-to-blocklist-12.png)

1. 「**[!UICONTROL 今すぐ実行]**」を選択し、「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/add-person-to-blocklist-13.png)

1. 「**[!UICONTROL 実行]**」をもう一度クリックします。

   ![](assets/add-person-to-blocklist-14.png)

これらのユーザーにはメールが送信されません。

>[!TIP]
>
>**Change Data Value**&#x200B;を使用して[トリガーキャンペーン &#x200B;](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md){target="_blank"}を作成し、**Block Listed is true**&#x200B;を指定して、個のセグメントを作成できます。これは、将来作成できる属性を持つすべてのユーザーに対して適用されます。
