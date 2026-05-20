---
unique-page-id: 1146942
description: トリガースマートキャンペーンのスマートリストを定義する方法を説明します。 トリガーの対象となるフィルタを設定します。
title: スマートキャンペーン用スマートリストの定義 |トリガー
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/QUFO9gKc3-1Pla-Shhy0Ns9pfcQKA3J8YFiYOSMIdgY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 92%

---

# スマートキャンペーン用スマートリストの定義 |トリガー {#define-smart-list-for-smart-campaign-trigger}

トリガーを追加して、ライブイベントに基づいて一度に 1 人ずつスマートキャンペーンを実行するようにします。

>[!CAUTION]
>
>アクティブなキャンペーンに対してスマートリストまたはフローステップの編集を行うと、その機能が損なわれる可能性があります。 その場合は、慎重に作業を進めてください。

1. スマートキャンペーンで、「**[!UICONTROL スマートリスト]**」タブをクリックします。

   ![](assets/define-smart-list-for-smart-campaign-trigger-1.png)

1. 目的のトリガーを検索し、キャンバスにドラッグ＆ドロップします。

   ![](assets/define-smart-list-for-smart-campaign-trigger-2.png)

   >[!NOTE]
   >
   >トリガーを使用したスマートキャンペーンは、_トリガー_&#x200B;モードで実行されます。 トリガーされたイベントと追加された任意のフィルターに基づいて、1 人につき一度ずつ実行されます。

   >[!IMPORTANT]
   >
   >トリガーキャンペーンスマートリストで、ブーリアンフィールドを使用する場合、キャンペーンの実行中にフィールドが正しく評価されるように、明示的に「false」に設定する必要があります。

1. ドロップダウンをクリックし、演算子を選択します。

   ![](assets/define-smart-list-for-smart-campaign-trigger-3.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報が見つからないことを示します。 修正されない場合、キャンペーンは無効になり、実行されません。

   >[!TIP]
   >
   >トリガーとフィルターの両方を持つスマートキャンペーンでは、トリガーが一番上に表示され、トリガーされると、フィルター条件を満たす人物のみがフローを通過します。

1. トリガーを定義します。

   ![](assets/define-smart-list-for-smart-campaign-trigger-4.png)

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、_いずれかの_&#x200B;トリガーがアクティブ化すると、フローに進みます。

一連のリードに対してキャンペーンを同時に実行するには、[スマートキャンペーンのスマートリストを定義する | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}を参照してください。

>[!MORELIKETHIS]
>
>[スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}
