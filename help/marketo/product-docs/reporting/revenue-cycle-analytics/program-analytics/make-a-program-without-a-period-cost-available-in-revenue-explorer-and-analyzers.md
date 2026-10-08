---
unique-page-id: 2360389
description: Marketo EngageのRevOpsおよびアナライザーで、期間費用なしでプログラムを作成する方法を説明します。 このガイドを使用して、次のステップを完了してください。
title: 期間原価がないプログラムを収益エクスプローラーとアナライザーで使用可能にする
exl-id: 45a24b9f-d92f-4f48-a7d1-0be14cd128b1
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
source-wordcount: '260'
ht-degree: 90%
---
# 期間原価がないプログラムを収益エクスプローラーとアナライザーで使用可能にする {#make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers}

プログラム期間原価を使用すると、プログラムの「金額」と「タイミング」を定義できます。 これは、収益サイクルエクスプローラーと[アナライザー](/help/marketo/product-docs/reporting/revenue-cycle-analytics/opportunity-influence-analyzer/tell-the-marketing-story-with-an-opportunity-influence-analyzer.md)に表示されます。

>[!NOTE]
>
>**管理者権限が必要**

期間コストがない場合でも、一部のプログラムを含める必要がある場合があります。 期間コストには 0 を入力できますが、これらのプログラムをより簡単に含めることができるようになりました。

>[!NOTE]
>
>プログラムアナライザーは、期間コスト別にプログラムの成功を区分します。 期間コストがない場合、プログラムの分析動作に関係なく、プログラムの成功は表示されません。 分析動作が設定されている場合、商談指標（パイプラインの商談、獲得した収益など）のデータが表示されます。

1. 「[!UICONTROL 管理]」セクションで「**[!UICONTROL タグ]**」をクリックします。

   ![](assets/image2014-9-17-12-3a35-3a32.png)

1. チャネルを展開し、目的のチャネルをダブルクリックします。

   >[!NOTE]
   >
   >このチャネルを使用するすべてのプログラムは、期間コストの有無に関係なく、収益エクスプローラーとアナライザーで利用できるようになります。 この変更は翌日に有効になります。

   ![](assets/image2014-9-17-12-3a36-3a7.png)

1. [!UICONTROL 分析の動作]を&#x200B;**包括的**&#x200B;に変更し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2014-9-17-12-3a36-3a13.png)

>[!TIP]
>
>「オペレーショナル」オプションに気づきましたか？ これは逆です。 期間コストに関係なく、これらのプログラムは除外されます。

これで完了です。 変更されたチャネルを使用するプログラムは、期間コストなしで収益エクスプローラーおよびアナライザーに含まれるようになります。

>[!MORELIKETHIS]
>
>[プログラムレベルでの分析動作の上書き](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/override-analytics-behavior-at-the-program-level.md)
