---
unique-page-id: 2360421
description: Analytics ビヘイビアーの上書きなど、Marketo EngageのプログラムレベルでのAnalytics ビヘイビアーの上書きについて説明します。 自信を持って次のステップへ。
title: プログラムレベルでの分析動作の上書き
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
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
source-wordcount: '202'
ht-degree: 89%
---
# プログラムレベルでの分析の動作を上書き {#override-analytics-behavior-at-the-program-level}

[チャネルの管理者レベルでの分析動作](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md)を設定することができますが、プログラムレベルで上書きすることもできます。 その方法をご紹介します。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;領域に移動します。

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. プログラムを選択します。

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. 「**[!UICONTROL 設定]**」タブで、「[!UICONTROL 分析動作]」をキャンバスにドラッグします。

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. 必要な[!UICONTROL 分析動作]を選択します。

   >[!NOTE]
   >
   >**定義**
   >
   >* **包含** - このオプションを使用すると、期間原価が含まれているかどうかに関係なく、収益エクスプローラーおよびアナライザーでプログラムをレポートに表示できます。
   >* **オペレーショナル** - このオプションを選択すると、プログラムが収益エクスプローラーまたはアナライザーに表示されなくなります。

   >[!NOTE]
   >
   >デフォルトの動作（この設定が適用されていない場合）は **1 つ以上の期間原価（0 ドルが割り当てられている期間も含む）がある**&#x200B;場合にのみ分析に含まれます。

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-24-11-3a42-3a6.png)

これで完了です。 これで、プログラムレベルで分析の動作を上書きする方法がわかりました。

>[!NOTE]
>
>変更は翌日に反映され、収益エクスプローラーおよびアナライザーを使用可能にするか、取り出されます。
