---
unique-page-id: 1146940
description: スマートキャンペーン用スマートリストの定義 |バッチ - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーン用スマートリストの定義 | バッチ
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 100%

---

# スマートキャンペーン用スマートリストの定義 | バッチ {#define-smart-list-for-smart-campaign-batch}

スマートリストは、レポート、リスト、スマートキャンペーンのどれであるかに関わらず、「誰」（どの人物）を含めるのかを定義する Marketo 全体のメカニズムです。バッチキャンペーンのスマートリストを定義する方法を次に示します。

1. スマートキャンペーンを選択し、「**スマートリスト**」をクリックします。

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 入力してフィルターを検索し、キャンバスにドラッグ＆ドロップします。同じ操作を複数のフィルターに対して繰り返します。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >フィルターのみのスマートキャンペーンは、**バッチ**&#x200B;モードで実行されます。適合するデータベース内の人物をフィルターに基づいて検索し、それらすべての人物に対して一度にフローを実行します。

   >[!NOTE]
   >
   >ライブイベントに基づいて 1 人ずつスマートキャンペーンを実行できるようにするには、トリガーを追加します。スマートキャンペーンは&#x200B;**トリガー**&#x200B;モードになります。

1. ドロップダウンをクリックし、選択したフィルターのフィルター演算子を選択します。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報が見つからないことを示します。修正されない場合、キャンペーンは無効になり、実行されません。

1. フィルター値を入力します。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >デフォルトでは、すべてのスマートリストルールを満たす人物が選定されます。これは、キャンペーンのニーズに合わせて変更できます。[複雑なロジックのスマートリストルール](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)を参照してください。

   ライブトリガーで 1 人ずつイベントを作成するには、[スマートキャンペーン用スマートリストの定義 | トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
