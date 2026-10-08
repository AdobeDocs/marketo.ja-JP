---
unique-page-id: 4718672
description: Marketo Engageで収益モデルのトランジションを使用して、収益モデルのトランジションを使用する方法を説明します。 このガイドを使用して、次のステップを完了してください。
title: 収益モデルのトランジションを使用する
exl-id: c658b631-b849-438a-b412-63ffd41e4c85
feature: Reporting, Revenue Cycle Analytics
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
    internal-label: Reporting
  - id: 126e34f9-e02a-505e-9978-ea36537f3ef9
    internal-label: Revenue Cycle Analytics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 73%
---
# 収益モデルのトランジションを使用する {#using-revenue-model-transitions}

>[!PREREQUISITES]
>
>[収益モデルの新規作成](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/create-a-new-revenue-model.md)

モデルを作成し、在庫ステージを選択して整理したら、次は移行を設定します。

![](assets/one-2.png)

1. 矢印の 1 つを右クリック（ダブルクリックも可能）し、「**[!UICONTROL トランジションを編集]**」を選択します。

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >「[!UICONTROL 匿名]⇒[!UICONTROL 既知]」トランジションルールは編集できません。

1. 選択したトランジションについて、新しいタブが開きます。

   ![](assets/three-1.png)

1. トランジションは、リードがステージ間をどのように移動するかを制御します。 右側から選択したトリガー（またはフィルター）をドラッグし、キャンバス上で放します。 この例では、「**[!UICONTROL フォームへの記入]**」トリガーを選択します。

   >[!TIP]
   >
   >収益モデラがレポート用に設定されているので、トリガーを常に含めることをお勧めします。 そうすれば、モデルとステージフローの真の速度がレポートに反映されます。 フィルターをトリガーと共に追加して、追加の制約を設定できます。

   ![](assets/four-2.png)

1. 選択したトリガーまたはフィルターのパラメーターを選択します。

   ![](assets/five-2.png)

1. モデルに戻るには、「**[!UICONTROL Modeler]**」をクリックします。

   ![](assets/six.png)

1. 画面の下部に、トランジションのルールが表示されます。

   ![](assets/seven.png)

1. すべてのトランジションについてルールを設定したら、「**[!UICONTROL 認証]**」をクリックして検証します。

   ![](assets/eight.png)

1. 検証で問題がなければ、以下のメッセージが表示されます。

   ![](assets/nine.png)

お疲れ様です。 モデルのトランジションが正常に変更されました。

>[!MORELIKETHIS]
>
>[収益モデルの承認／未承認](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/approve-unapprove-a-revenue-model.md)
