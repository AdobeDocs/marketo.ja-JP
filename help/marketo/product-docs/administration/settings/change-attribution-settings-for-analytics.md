---
unique-page-id: 2360217
description: 収益サイクル分析で、ファーストタッチとマルチタッチのアトリビューション、リードコンバージョン、マーケティングの影響を受けた機会オプションを設定する方法。
title: 分析用属性設定の変更
exl-id: 4740b0fa-ddaf-46ed-87d6-8b3f8d35afe3
feature: Administration
TQID: https://experienceleague.adobe.com/AjpEYRzLKRQQsTmYdQUvAVnlcmG-Q6nbVjaZCuQYaUc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: e5d29014-8a81-4c0c-845b-2adc7a5d6258
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 79%

---

# 分析用属性設定の変更 {#change-attribution-settings-for-analytics}

ファーストタッチおよびマルチタッチのアトリビューションの商談、リードコンバージョン指標、マーケティングが影響を与えた商談フラグに、Marketo が連絡先を結び付ける方法を変更できます。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/change-attribution-settings-for-analytics-1.png)

1. 「**[!UICONTROL 収益サイクル分析]**」をクリックします。

   ![](assets/change-attribution-settings-for-analytics-2.png)

1. 「**[!UICONTROL アトリビューション]**」で、「**[!UICONTROL 編集]**」リンクをクリックします。

   ![](assets/change-attribution-settings-for-analytics-3.png)

   >[!TIP]
   >
   >この設定を変更しても、Marketo データは変更されません。レポートの実行方法が変更されます。 この設定は、いつでも元に戻すことができます。

1. オプションを選択し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/change-attribution-settings-for-analytics-4.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**[!UICONTROL 明示的]**：ロールのある取引先責任者のみ（デフォルト）。
   >
   >**[!UICONTROL 混合]**：ロールのある取引先責任者（ある場合）。 使用できる連絡先がない場合は、アカウント内のすべての連絡先が使用されます。
   >
   >**[!UICONTROL 暗黙的]**：ロールを問わずすべての取引先責任者。

>[!CAUTION]
>
>**[!UICONTROL 暗黙的]**&#x200B;を使用する場合、Marketo は常に、ロールに関係なく、アカウントに関連付けられたすべての連絡先を調べます。 **Marketo では、[!UICONTROL 明示的]モードの使用を強くお勧めします**。 [!UICONTROL 暗黙的]モードを使用すると、商談に実際の影響を与えないにもかかわらず、商談に対してクレジットを持つ人物という偽陽性を生み出す可能性があります。 [!UICONTROL 暗黙的]モードは慎重に使用してください。
