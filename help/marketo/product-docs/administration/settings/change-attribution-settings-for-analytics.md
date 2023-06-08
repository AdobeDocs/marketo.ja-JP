---
unique-page-id: 2360217
description: 分析用アトリビューション設定の変更 - Marketo ドキュメント - 製品ドキュメント
title: 分析用アトリビューション設定の変更
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
source-git-commit: b71729a678ff4a676bb60803d845d0a44118f7e5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 69%

---

# 分析用アトリビューション設定の変更 {#change-attribution-settings-for-analytics}

ファーストタッチおよびマルチタッチのアトリビューションの商談、リードコンバージョン指標、マーケティングが影響を与えた商談フラグに、Marketo が連絡先を結び付ける方法を変更できます。

これらの設定は、次に影響します： [!UICONTROL 収益エクスプローラ] レポート [プログラム商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md), [商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)、およびリード分析領域 これは、 [!UICONTROL プログラムアナライザ] レポート。

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
>**[!UICONTROL 暗黙的]**&#x200B;を使用する場合、Marketo は常に、ロールに関係なく、アカウントに関連付けられたすべての連絡先を調べます。**Marketo [!UICONTROL 明示] mode**. 使用 [!UICONTROL 暗黙] は偽陽性を作り出す可能性がある。つまり、オポチュニティに実際の影響を与えていないにもかかわらず、オポチュニティに対するクレジットを持つ人。 用途 [!UICONTROL 暗黙] 注意して
