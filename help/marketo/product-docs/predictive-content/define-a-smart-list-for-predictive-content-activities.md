---
unique-page-id: 10097873
description: 予測コンテンツアクティビティのためのスマートなリストの定義 — Marketto Docs — 製品ドキュメント
title: 予測コンテンツアクティビティのためのスマートリストの定義
translation-type: tm+mt
source-git-commit: f1d7b270454ba41db5197a069e0dcc2caebdec63
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---


# 予測コンテンツアクティビティ用のスマートリストの定義{#define-a-smart-list-for-predictive-content-activities}

スマートキャンペーンでスマートリストを定義する際に、トリガーやフィルターで予測コンテンツアクティビティを使用できます。 [リッチメディアテンプレート](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[コンテンツレコメンデーションバー](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)、または[電子メール](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md)を使用して、予測コンテンツをクリックしたユーザーに対するアクションをトリガーできます。

1. スマートキャンペーンで、「**スマートリスト**」タブに移動します。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >賢いリストは素晴らしい事をできます 詳しくは、[スマートリストディープダイブ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を参照してください。

1. トリガーを検索し、キャンバスにドラッグ&amp;ドロップします。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >トリガーを持つスマートキャンペーンは、トリガーモードで実行されます。 このイベントは、トリガーされたイベントと追加されたフィルターに基づいて、一度に1人のユーザーに対して実行されます。

1. **名前**&#x200B;ドロップダウンをクリックし、演算子を選択します。

   ![](assets/smart-list-dropdown-hands.png)

1. トリガーを定義します。

   ![](assets/smart-lislt-select-content-hands.png)

1. 追加&#x200B;**型**&#x200B;制約。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. スマートリストに必要なソースを選択します。

   ![](assets/pc-add-constraint.png)

1. 予測コンテンツに電子メールソースを使用している場合は、「電子メール&#x200B;**」トリガーに**「リンクをクリック」を追加します。 電子メールを選択し、**true**&#x200B;として定義された&#x200B;**Is Predictive**&#x200B;制約を追加します。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 必要に応じ追加て、その他のフィルター。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >トリガーとフィルターの両方があるスマートキャンペーンでは、トリガーが一番上に表示されます。 トリガーされると、フィルター条件を満たすユーザーのみがフローを通過します。

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、トリガーのいずれか1つが有効になると、人はフローに入ります。

   一連のユーザーに対してキャンペーンを同時に実行するには、[バッチスマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)のスマートリストを定義する方法を学びます。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーンのスマートリストの定義 |バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [スマ追加ートキャンペーンへのフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Webパーソナライゼーションアクティビティ用のスマートリストの定義](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Webリッチメディアの予測コンテンツを有効にする](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [コンテンツレコメンデーションバーの有効化](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

