---
unique-page-id: 2360217
description: 分析用アトリビューション設定の変更 - Marketo ドキュメント - 製品ドキュメント
title: 分析用アトリビューション設定の変更
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 100%

---

# 分析用アトリビューション設定の変更 {#change-attribution-settings-for-analytics}

ファーストタッチおよびマルチタッチのアトリビューションの商談、リードコンバージョン指標、マーケティングが影響を与えた商談フラグに、Marketo が連絡先を結び付ける方法を変更できます。

これらの設定は、[プログラム商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)、[商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)、リード分析の各領域で、収益エクスプローラーレポートに影響を与えます。また、プログラムアナライザーレポートにも影響を与えます。

1. 「**管理者**」領域に移動します。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 「**収益サイクルアナリティクス**」をクリックします。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 「**アトリビューション**」で、「**編集**」リンクをクリックします。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >この設定を変更しても、Marketo のデータは変更されません。単に、レポートの実行方法を変更するだけです。この設定は、いつでも元に戻すことができます。

1. オプションを選択し、「**保存**」をクリックします。

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**明示的**：役割のある取引先責任者のみ（デフォルト）。
   >
   >**混合**：役割のある取引先責任者（ある場合）。使用できる連絡先がない場合は、アカウント内のすべての連絡先が使用されます。
   >
   >**暗黙的**：役割を問わずすべての取引先責任者。

>[!CAUTION]
>
>**暗黙的**&#x200B;を使用する場合、Marketo は常に、役割に関係なく、アカウントに関連付けられたすべての連絡先を調べます。**Marketo では明示的モードの使用を強くお勧めします**。暗黙的モードを使用すると、商談に実際の影響を与えないにもかかわらず、商談に対してクレジットを持つ人という偽陽性を生み出す可能性があります。暗黙的モードは慎重に使用してください。
