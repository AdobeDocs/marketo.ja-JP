---
unique-page-id: 8782266
description: web キャンペーンの優先順位付けなど、Marketo Engageでのweb キャンペーンの優先順位付けについて説明します。 このガイドを使用して、次のステップを完了してください。
title: Web キャンペーンの優先順位付け
exl-id: 18c43ba2-6d4a-4344-93be-3e1435742504
feature: Web Personalization
TQID: 'https://experienceleague.adobe.com/MwSVFrnnG-tBShEwxhapBPm0evix-J0ZbrgvWwBZSU8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
    internal-label: Personalization
  - id: 664d862c-1673-5ed4-a3d6-386ac83225e4
    internal-label: Web Personalization
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 89%
---
# Web キャンペーンの優先順位付け {#prioritizing-web-campaigns}

優先度スコアを設定して、2 つ以上の Web キャンペーンが重複する場合に Web キャンペーンを優先します。

>[!NOTE]
>
>**重複するキャンペーン**
>
>Web キャンペーンの重複は、以下の場合に発生します。
>
>* 複数のウィジェットキャンペーンやダイアログキャンペーンが、同じページで同時に表示される場合
>* 同じゾーン ID を持つ複数の In Zone が、同じ web ページで同時に表示される場合
>
>ゾーン内キャンペーンと（ウィジェットまたはダイアログ）キャンペーンが、同じページで表示されることもあります。

1. 「**[!UICONTROL Web キャンペーン]**」に移動します

   ![](assets/web-campaigns-hand-6.jpg)

   >[!NOTE]
   >
   >目的の web キャンペーンを見つけやすくするには、[フィルター機能](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/filter-web-campaigns.md)を使用します。

1. キャンペーンを編集ページで、「[!UICONTROL 優先度スコア]」（9999 =最も高い優先度、1 =最も低い優先度）を設定します。

   ![](assets/image2015-7-9-20-3a20-3a58.png)

   >[!TIP]
   >
   >キャンペーンの[!UICONTROL 優先度スコア]は、キャンペーンの重複が生じる可能性があり、いずれかのキャンペーンの重要度が高い場合にのみ使用することをお勧めします。 すべてのキャンペーンに優先度を設定する必要はありません。

1. キャンペーンを保存または起動します。

1. [!UICONTROL Web キャンペーン]ページに表示される[!UICONTROL 優先度スコア]を参照してください。

![](assets/web-campaign-priority-score.jpg)
