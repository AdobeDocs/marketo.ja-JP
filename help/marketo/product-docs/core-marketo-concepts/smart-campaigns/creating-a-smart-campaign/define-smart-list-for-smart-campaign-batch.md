---
unique-page-id: 1146940
description: スマートキャンペーン用スマートリストの定義 |バッチ - Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーン用スマートリストの定義 | バッチ
exl-id: 0e0061a9-df24-4cf6-8f1e-09ff0ee62efa
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 100%

---

# スマートキャンペーン用スマートリストの定義 | バッチ {#define-smart-list-for-smart-campaign-batch}

スマートリストは、Marketo 全体で、レポート、リスト、スマートキャンペーンのどれであるかに関わらず、「誰」（どの人物）を含めるのかを定義するメカニズムです。バッチキャンペーンのスマートリストを定義する方法を次に示します。

1. スマートキャンペーンを選択し、「**スマートリスト**」をクリックします。

   ![](assets/campaignchoose-hand.png)

1. フィルターを入力して検索し、それをキャンバスにドラッグ＆ドロップします。複数のフィルターに対して繰り返します。

   ![](assets/dragin.png)

   >[!NOTE]
   >
   >フィルターのみのスマートキャンペーンは、**バッチ**&#x200B;モードで実行されます。フィルターに基づいて適合するデータベース内の人物を検索し、それらすべての人に対して一度にフローを実行します。

   >[!NOTE]
   >
   >ライブイベントに基づいて、一度に 1 人ずつスマートキャンペーンを実行できるようにするには、トリガーを追加します。スマートキャンペーンが&#x200B;**トリガー**&#x200B;モードになります。

1. ドロップダウンをクリックし、選択したフィルターのフィルター演算子を選択します。

   ![](assets/programdropdown-hands.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報が見つからないことを示します。修正されない場合、キャンペーンは無効になり、実行されません。

1. フィルター値を入力します。

   ![](assets/chooseprogram.png)

   >[!NOTE]
   >
   >デフォルトでは、すべてのスマートリストルールを満たす人物が選定されます。これは、キャンペーンのニーズに合わせて変更できます。[複雑なロジックのスマートリストルール](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)を参照してください。

   ライブトリガーで 1 人ずつイベントを作成するには、[スマートキャンペーン用スマートリストの定義 | トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

