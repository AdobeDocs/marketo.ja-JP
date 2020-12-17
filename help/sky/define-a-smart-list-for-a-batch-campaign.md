---
title: define-a-smart-リスト-for-a-batch-キャンペーン
description: バッチキャンペーンのスマートリストの定義
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---


# バッチキャンペーンのスマートリストの定義

<br> 

スマートリストは、レポート、リスト、スマートキャンペーンのいずれを含めるかを定義する、マーケティング全体のメカニズムです。 バッチキャンペーンのスマートリストを定義する方法を次に示します。

1. スマートキャンペーンを選択し、[**[!UICONTROL スマートリスト]**]をクリックします。

   ![イメージ1](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-1.png)

1. フィルターを検索するには、と入力し、カンバスにドラッグ&amp;ドロップします。 複数のフィルターに対して同じ手順を繰り返します。

   ![イメージ2](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-2.png)

   >[!NOTE]
   >
   >フィルターのみを持つスマートキャンペーンは、バッチモードで実行されます。 データベース内でフィルターに基づいて認定を受ける人を見つけ、そのすべてを一度にフローを通じて実行します。

   >[!IMPORTANT]
   >
   >スマートキャンペーンをトリガーモードにするトリガーを追加することで、ライブイベントに基づいて、一度に1人の人に対してスマートキャンペーンを実行させることができます。

1. ドロップダウンをクリックし、フィルター演算子(例：選択したフィルターの&#x200B;**[!UICONTROL は]**、**[!UICONTROL は]**&#x200B;ではありません（など）。

   ![イメージ3](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-3.png)

   >[!CAUTION]
   >
   >赤い線はエラーを示しているか、情報が見つからないことを示しています。 修正しないと、キャンペーンは無効になり、実行されません。

1. フィルタ値を入力します。

   ![画像4](/help/sky/assets/smart-campaigns/define-a-smart-list-for-a-batch-campaign/define-a-smart-list-for-a-batch-campaign-4.png)

>[!NOTE]
>
>デフォルトでは、すべてのスマートリストルールを満たすユーザーは
>資格を持つ これは、キャンペーンのニーズに合わせて変更できます。 詳しくは、[複雑なロジックのスマートリストルール](https://docs.marketo.com/display/DOCS/Using+Advanced+Smart+List+Rule+Logic)を参照してください。
>
>1人ずつライブイベント上でトリガーするには、[スマートキャンペーン用のスマートリストを定義する方法を学びます。 |トリガー](https://docs.marketo.com/display/DOCS/Define+Smart+List+for+Smart+Campaign+%7C+Trigger)。
