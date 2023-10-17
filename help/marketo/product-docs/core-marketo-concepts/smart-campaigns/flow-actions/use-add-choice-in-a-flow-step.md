---
unique-page-id: 1146980
description: フローステップでの「選択肢を追加」の使用 - Marketo ドキュメント - 製品ドキュメント
title: フローステップでの「選択肢を追加」の使用
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 71%

---

# フローステップでの「選択肢を追加」の使用 {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

「選択肢を追加」では、フローステップを使用し、詳細を選択する際に「依存」と言うことができます。

1. の下 **[!UICONTROL 流量]** スマートキャンペーンの「 」タブで、フローステップを追加して、 **[!UICONTROL 選択肢を追加]**.

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. 選択肢の条件を選択します。

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. 選択肢の演算子を選択して、値を入力します。これにより基準すなわち選択肢が設定されます。

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. 選択肢のフローステップ値を入力します。

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >選択肢のフローステップの条件部分では、トークンは正しく&#x200B;_機能しません_。

1. 上記の手順を繰り返して複数の選択肢を追加したら、デフォルト値を追加／調整します。

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >その選択肢に対して何も実行したくなければ、フローステップを「--何もしない--」に設定することも可能です。

   >[!CAUTION]
   >
   >フローステップに適用されるのは、最初に一致した選択肢だけです。[フローアクションの「選択肢を追加」の並べ替え](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}を参照してください。

   完了です。各選択に対して複数のスマートキャンペーンを作成する代わりに、フローステップの選択肢を含む 1 つのスマートキャンペーンを作成できるようになりました。

   >[!MORELIKETHIS]
   >
   >[フローステップの「選択肢を追加」の並べ替え](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md){target="_blank"}
