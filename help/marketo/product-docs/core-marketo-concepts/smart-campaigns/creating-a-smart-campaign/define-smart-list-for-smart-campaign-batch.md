---
unique-page-id: 1146940
description: スマートキャンペーン用スマートリストの定義 |バッチ - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーン用スマートリストの定義 | バッチ
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
feature: Smart Campaigns
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 90%

---

# スマートキャンペーン用スマートリストの定義 | バッチ {#define-smart-list-for-smart-campaign-batch}

スマートリストは、Marketo Engage全体のメカニズムで、レポート、リスト、スマートキャンペーンのどれであるかに関わらず、「誰」（どのユーザー）を含めるかを定義できます。 バッチキャンペーンのスマートリストを定義する方法を次に示します。

1. スマートキャンペーンを選択し、「**[!UICONTROL スマートリスト]**」をクリックします。

   ![](assets/define-smart-list-for-smart-campaign-batch-1.png)

1. 入力してフィルターを検索し、キャンバスにドラッグ＆ドロップします。同じ操作を複数のフィルターに対して繰り返します。

   ![](assets/define-smart-list-for-smart-campaign-batch-2.png)

   >[!NOTE]
   >
   >フィルターのみのスマートキャンペーンは、_バッチ_&#x200B;モードで実行されます。適合するデータベース内の人物をフィルターに基づいて検索し、それらすべての人物に対して一度にフローを実行します。

   >[!NOTE]
   >
   >ライブイベントに基づいて 1 人ずつスマートキャンペーンを実行できるようにするには、トリガーを追加します。スマートキャンペーンは&#x200B;_トリガー_&#x200B;モードになります。

1. ドロップダウンをクリックし、選択したフィルターのフィルター演算子を選択します。

   ![](assets/define-smart-list-for-smart-campaign-batch-3.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報が見つからないことを示します。修正されない場合、キャンペーンは無効になり、実行されません。

1. フィルター値を入力します。

   ![](assets/define-smart-list-for-smart-campaign-batch-4.png)

   >[!NOTE]
   >
   >デフォルトでは、すべてのスマートリストルールを満たす人物が選定されます。これは、キャンペーンのニーズに合わせて変更できます。[複雑なロジックのスマートリストルール](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}を参照してください。

   ライブトリガーで 1 人ずつイベントを作成するには、[スマートキャンペーン用スマートリストの定義 | トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
