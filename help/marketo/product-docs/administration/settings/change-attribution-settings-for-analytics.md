---
unique-page-id: 2360217
description: 分析用属性設定の変更 - Marketo ドキュメント - 製品ドキュメント
title: 分析用属性設定の変更
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: ht
source-wordcount: '189'
ht-degree: 100%

---

# 分析用属性設定の変更 {#change-attribution-settings-for-analytics}

ファーストタッチおよびマルチタッチのアトリビューションの商談、リードコンバージョン指標、マーケティングが影響を与えた商談フラグに、Marketo が連絡先を結び付ける方法を変更できます。

これらの設定は、[プログラム商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)、[商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)、リード分析の各領域にある[!UICONTROL 売上高エクスプローラー]レポートに影響を与えます。また、[!UICONTROL プログラムアナライザー]レポートにも影響を与えます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 「**[!UICONTROL 収益サイクルアナリティクス]**」をクリックします。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 「**[!UICONTROL アトリビューション]**」で、「**[!UICONTROL 編集]**」リンクをクリックします。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >この設定を変更しても、Marketo のデータは変更されません。単に、レポートの実行方法を変更するだけです。この設定は、いつでも元に戻すことができます。

1. オプションを選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL 明示的]**：ロールのある取引先責任者のみ（デフォルト）。
   >
   >**[!UICONTROL 混合]**：ロールのある取引先責任者（ある場合）。使用できる連絡先がない場合は、アカウント内のすべての連絡先が使用されます。
   >
   >**[!UICONTROL 暗黙的]**：ロールを問わずすべての取引先責任者。

>[!CAUTION]
>
>**[!UICONTROL 暗黙的]**&#x200B;を使用する場合、Marketo は常に、ロールに関係なく、アカウントに関連付けられたすべての連絡先を調べます。**Marketo では、[!UICONTROL 明示的]モードの使用を強くお勧めします**。[!UICONTROL 暗黙的]モードを使用すると、商談に実際の影響を与えないにもかかわらず、商談に対してクレジットを持つ人物という偽陽性を生み出す可能性があります。[!UICONTROL 暗黙的]モードは慎重に使用してください。
