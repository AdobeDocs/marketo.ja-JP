---
unique-page-id: 10097873
description: 予測コンテンツアクティビティのためのスマートなリストの定義 — Marketto Docs — 製品ドキュメント
title: 予測コンテンツアクティビティのためのスマートリストの定義
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# 予測コンテンツアクティビティのためのスマートリストの定義 {#define-a-smart-list-for-predictive-content-activities}

>[!NOTE]
>
>購入日に応じて、マーケティング担当購読に「予測コンテンツ」または「コンテンツ`<sup>AI</sup>`」が含まれる場合があります。 予測コンテンツを使用するユーザーの場合、Marketing Cloudでは、2018年4月31日までコンテンツ`<sup>AI</sup>` 分析機能を有効にしています。 これらの機能をこの日以降に引き続きご利用いただくには、マーケティング担当者カスタマーサクセスマネージャーにお問い合わせの上、マーケティングコンテンツにアップグレードしてください`<sup>AI</sup>`。

スマートキャンペーンでスマートリストを定義する際に、トリガーおよびフィルターで予測コンテンツアクティビティを使用できます。 リッチメディアテンプレート [、](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)コンテンツレコメンデーションバー [](enabling-predictive-content/enable-the-content-recommendation-bar.md)、電子メール内で、予測コンテンツをクリックするすべての人に対してアクションをトリガーできます。

1. スマート・キャンペーンで、「 **スマート・リスト** 」タブに移動します。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >**ディープダイブ**
   >
   >
   >賢いリストは素晴らしい事をできます 詳しくは、 [スマートリストの詳細を参照してください](../../product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)。

1. トリガーを検索し、キャンバスにドラッグ&amp;ドロップします。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >トリガーを持つスマートキャンペーンは、トリガーモードで実行されます。 このイベントは、トリガーされたイベントと追加されたフィルターに基づいて、一度に1人のユーザーに対して実行されます。

1. 「 **名前** 」ドロップダウンをクリックし、演算子を選択します。

   ![](assets/smart-list-dropdown-hands.png)

1. トリガーを定義します。

   ![](assets/smart-lislt-select-content-hands.png)

1. 追加 **Type** 制約。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. スマートリストに必要なソースを選択します。

   ![](assets/pc-add-constraint.png)

1. 予測コンテンツに電子メールソースを使用している場合は、「電子メール**トリガー」に**Clicksリンクを追加します。 電子メールを選択し、「 **Is Predictive** 」制約( **trueと定義)を追加します**。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 必要に応じ追加て、その他のフィルター。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >トリガーとフィルターの両方を備えたスマートキャンペーンでは、トリガーが一番上に表示されます。 トリガーされると、フィルター条件を満たすユーザーのみがフローを通過します。

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、ONE theトリガーがアクティブ化されると、個人がフローに入ります。

   [バッチスマートキャンペーンのスマートリストの定義](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)

   >[!NOTE]
   >
   >**関連記事**
   >
   >    
   >    
   >    * [スマートキャンペーンのスマートリストの定義 |バッチ](../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >    * [スマ追加ートキャンペーンへのフローステップ](../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >    * [Webパーソナライゼーションアクティビティ用のスマートリストの定義](../../product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >    * [Webリッチメディアの予測コンテンツを有効にする](enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >    * [コンテンツレコメンデーションバーの有効化](enabling-predictive-content/enable-the-content-recommendation-bar.md)


一連のユーザーに対してキャンペーンを同時に実行するには、の方法を学習します。