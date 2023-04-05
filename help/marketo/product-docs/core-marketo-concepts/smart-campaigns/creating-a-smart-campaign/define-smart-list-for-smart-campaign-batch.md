---
unique-page-id: 1146940
description: スマートキャンペーン用スマートリストの定義 |バッチ - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーン用スマートリストの定義 | バッチ
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 56d3d05d5462c79f32f507655266e3bfa0cc6846
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 57%

---

# スマートキャンペーン用スマートリストの定義 | バッチ {#define-smart-list-for-smart-campaign-batch}

スマートリストは、Marketo全体で、レポート、リスト、スマートキャンペーンのどれであるかに関わらず、「誰」（どのユーザー）を含めるかを定義するメカニズムです。 バッチキャンペーンのスマートリストを定義する方法を次に示します。

1. スマートキャンペーンを選択し、 **スマートリスト**.

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 「 」と入力してフィルターを検索し、キャンバスにドラッグ&amp;ドロップします。 複数のフィルターに対して繰り返します。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >フィルターのみのスマートキャンペーンは、 **バッチ** モード。 フィルターに基づいて適合するデータベース内の人物を検索し、それらすべての人に対して一度にフローを実行します。

   >[!NOTE]
   >
   >スマートキャンペーンをライブイベントに基づいて一度に 1 人のユーザーに対して実行させる場合は、トリガーを追加します。追加すると、スマートキャンペーンが **トリガー** モード。

1. ドロップダウンをクリックし、選択したフィルターのフィルター演算子を選択します。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報が見つからないことを示します。修正されない場合、キャンペーンは無効になり、実行されません。

1. フィルター値を入力します。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >デフォルトでは、すべてのスマートリストルールを満たす担当者が選定されます。 これは、キャンペーンのニーズに合わせて変更できます。[複雑なロジックのスマートリストルール](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)を参照してください。

   ライブトリガーで 1 人ずつイベントを作成するには、[スマートキャンペーン用スマートリストの定義 | トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

