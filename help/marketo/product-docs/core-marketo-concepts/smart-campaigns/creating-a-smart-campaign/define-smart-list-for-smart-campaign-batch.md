---
unique-page-id: 1146940
description: スマートキャンペーンのスマートリストの定義 |バッチ —Marketoドキュメント — 製品ドキュメント
title: スマートキャンペーンのスマートリストの定義 |バッチ
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# スマートキャンペーンのスマートリストの定義 |バッチ{#define-smart-list-for-smart-campaign-batch}

スマートリストは、Marketo全体のメカニズムで、レポート、リスト、スマートキャンペーンのいずれであれ、誰を含めるかを定義するメカニズムです。 バッチキャンペーンのスマートリストを定義する方法を次に示します。

1. スマートキャンペーンを選択し、[**スマートリスト**]をクリックします。

   ![](assets/campaignchoose-hand.png)

1. フィルターを検索するには、と入力し、カンバスにドラッグ&amp;ドロップします。 複数のフィルターに対して同じ手順を繰り返します。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >フィルターのみのスマートキャンペーンは、**バッチ**&#x200B;モードで実行されます。 データベース内でフィルターに基づいて認定を受ける人を見つけ、そのすべてを一度にフローを通じて実行します。

   >[!NOTE]
   >
   >スマートキャンペーンを&#x200B;**トリガー**&#x200B;モードにするトリガーを追加することで、ライブイベントに基づいて一度に1人の人に対してスマートキャンペーンを実行させることができます。

1. ドロップダウンをクリックし、選択したフィルターのフィルター演算子を選択します。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報がないことを示します。 修正しないと、キャンペーンは無効になり、実行されません。

1. フィルタ値を入力します。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >デフォルトでは、すべてのスマートリストルールを満たすユーザーが資格を持ちます。 これは、キャンペーンのニーズに合わせて変更できます。 詳しくは、[複雑なロジックのスマートリストルール](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)を参照してください。

   1人ずつライブイベントをトリガーするには、[スマートキャンペーン用のスマートリストを定義する方法を学びます。 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーンのスマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [スマ追加ートキャンペーンへのフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

