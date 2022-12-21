---
unique-page-id: 1146980
description: フローステップでの「選択肢を追加」の使用 - Marketo ドキュメント - 製品ドキュメント
title: フローステップでの「選択肢を追加」の使用
exl-id: 50ffcd60-48ee-4341-94d8-170c63bc9ecb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 100%

---

# フローステップでの「選択肢を追加」の使用 {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>[スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

「**選択肢を追加**」を使用すると、フローステップで「条件に応じた」詳細の選択が可能になります。

1. スマートキャンペーンの「**フロー**」タブで、任意のフローステップを追加し、「**選択肢を追加**」をクリックします。

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. 選択肢の条件を選択します。

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. 選択肢の演算子を選択して、値を入力します。これにより基準すなわち選択肢が設定されます。

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. 選択肢のフローステップ値を入力します。

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >選択肢のフローステップの条件部分では、トークンは正しく&#x200B;**機能しません**。

1. 上記の手順を繰り返して複数の選択肢を追加したら、デフォルト値を追加／調整します。

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >その選択肢に対して何も実行したくなければ、フローステップを「--何もしない--」に設定することも可能です。

   >[!CAUTION]
   >
   >フローステップに適用されるのは、最初に一致した選択肢だけです。[フローアクションの「選択肢を追加」の並べ替え](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md)を参照してください。

   これで完了です。選択肢ごとに複数のスマートキャンペーンを作ることなく、フローステップ選択肢を用いた単一のスマートキャンペーンを作成できました。

   >[!MORELIKETHIS]
   >
   >[フローステップの「選択肢を追加」の並べ替え](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/reorder-add-choice-in-a-flow-step.md)
