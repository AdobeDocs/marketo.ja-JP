---
unique-page-id: 2360217
description: Analyticsのアトリビューション設定の変更 — Marketto Docs — 製品ドキュメント
title: Analyticsのアトリビューション設定の変更
translation-type: tm+mt
source-git-commit: f79909ce8f2e37bf0748596774fe47ac03618696
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Analyticsのアトリビューション設定の変更{#change-attribution-settings-for-analytics}

ファーストタッチとマルチタッチのアトリビューション、リードコンバージョン指標、およびマーケティングの影響を受けるオポチュニティフラグに関する連絡先の関連付け方法を変更できます。

これらの設定は、[プログラム商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/understanding-the-program-opportunity-analysis-area.md)、[商談分析](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/understanding-opportunity-analysis-in-revenue-explorer.md)およびリードの分析領域の下の売上高エクスプローラレポートに影響を与えます。 これは、プログラムアナライザーレポートにも影響します。

1. 「**管理者**」セクションで、「**売上高サイクル分析**」をクリックします。

   ![](assets/image2014-9-24-11-3a55-3a19.png)

1. 「**アトリビューション**」の下の「**編集**」リンクをクリックします。

   ![](assets/image2014-9-24-11-3a56-3a33.png)

   >[!TIP]
   >
   >この設定を変更しても、マーケティング担当者のデータは変更されません。レポートの実行方法を変更するだけです。 この状態は、いつでも元に戻すことができます。

1. オプションを選択し、「**保存**」をクリックします。

   ![](assets/image2014-9-24-11-3a57-3a39.png)

   >[!NOTE]
   >
   >**定義**
   >
   >**明示的**:ロール（デフォルト）を持つ連絡先のみ。
   >
   >**ハイブリッド**:役割がある場合は、その役割の連絡先。使用できる連絡先がない場合は、アカウント内のすべての連絡先が使用されます。
   >
   >**暗黙的**:役割に関係なく、すべての連絡先。

>[!CAUTION]
>
>**暗黙的**&#x200B;を使用する場合、Marketorは、ロールに関係なく、常にアカウントに関連付けられたすべての連絡先を調べます。 **明示的モードの使用を強くお勧めします**。Implicitを使用すると、偽陽性が発生する場合があります。例えば、機会に実際に影響を与えないにもかかわらず、機会に対する信用を持つ人。 「暗黙的」は慎重に使用してください。
