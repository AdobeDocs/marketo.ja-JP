---
unique-page-id: 1146942
description: スマートキャンペーン用スマートリストの定義 |トリガー- Marketo ドキュメント - 製品ドキュメント
title: スマートキャンペーン用スマートリストの定義 |トリガー
exl-id: 14d9b15e-864a-47ef-8f39-3d65e6036a82
source-git-commit: a15a4b9bccb069b51186aac7b913008d15aa645e
workflow-type: ht
source-wordcount: '229'
ht-degree: 100%

---

# スマートキャンペーン用スマートリストの定義 |トリガー {#define-smart-list-for-smart-campaign-trigger}

トリガーを追加して、ライブイベントに基づいて一度に 1 人ずつスマートキャンペーンを実行するようにします。

1. スマートキャンペーンで、「**スマートリスト**」タブをクリックします。

   ![](assets/image2014-9-19-16-3a22-3a55.png)

1. トリガーを検索し、キャンバスにドラッグ&amp;ドロップします。

   ![](assets/image2014-9-19-16-3a23-3a24.png)

   >[!NOTE]
   >
   >トリガーを使用したスマートキャンペーンは、**トリガー**&#x200B;モードで実行されます。トリガーされたイベントと追加された任意のフィルターに基づいて、1 人につき一度ずつ実行されます。

   >[!IMPORTANT]
   >
   >トリガーキャンペーンスマートリストで、ブーリアンフィールドを使用する場合、キャンペーンの実行中にフィールドが正しく評価されるように、明示的に「false」に設定する必要があります。

1. ドロップダウンをクリックし、演算子を選択します。

   ![](assets/image2014-9-19-16-3a23-3a29.png)

   >[!CAUTION]
   >
   >赤い波線は、エラーまたは情報が見つからないことを示します。修正されない場合、キャンペーンは無効になり、実行されません。

   >[!TIP]
   >
   >トリガーとフィルターの両方を持つスマートキャンペーンでは、トリガーが一番上に表示され、トリガーされると、フィルター条件を満たす人物のみがフローに進みます。

1. トリガーを定義します。

   ![](assets/image2014-9-19-16-3a24-3a36.png)

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、**いずれかの**&#x200B;トリガーがアクティブ化すると、フローに進みます。

一連のリードに対してキャンペーンを同時に実行するには、[スマートキャンペーンのスマートリストを定義する | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)を参照してください。

>[!MORELIKETHIS]
>
>[スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
