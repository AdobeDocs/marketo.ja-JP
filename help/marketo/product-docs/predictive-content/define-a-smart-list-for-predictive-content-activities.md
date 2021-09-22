---
unique-page-id: 10097873
description: 予測コンテンツアクティビティのスマートリストの定義 - Marketo ドキュメント - 製品ドキュメント
title: 予測コンテンツアクティビティのスマートリストの定義
exl-id: 2c72b215-8c0b-48b4-8492-8e3fe832fae9
source-git-commit: ''
workflow-type: ht
source-wordcount: '300'
ht-degree: 100%

---

# 予測コンテンツアクティビティのスマートリストの定義 {#define-a-smart-list-for-predictive-content-activities}

スマートキャンペーンでスマートリストを定義するとき、「予測コンテンツ」の活動をトリガーとフィルターで使用できます。[リッチメディアテンプレート](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)、[コンテンツレコメンデーションバー](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)、または[メール](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-in-emails.md)を使用して、予測コンテンツをクリックするすべての人に対してアクションをトリガーできます。

1. スマートキャンペーンで、「**スマートリスト**」タブに移動します。

   ![](assets/smart-list-1.png)

   >[!NOTE]
   >
   >スマートリストはとても便利です。詳しくは、[スマートリストの詳細](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md)を参照してください。

1. トリガーを検索し、キャンバスにドラッグ&amp;ドロップします。

   ![](assets/smart-list-drag-trigger-hands.png)

   >[!NOTE]
   >
   >トリガーを使用したスマートキャンペーンは、トリガーモードで実行されます。トリガーされたイベントと追加されたフィルターに基づいて、1 人につき一度ずつ実行されます。

1. 「**名前**」ドロップダウンをクリックし、演算子を選択します。

   ![](assets/smart-list-dropdown-hands.png)

1. トリガーを定義します。

   ![](assets/smart-lislt-select-content-hands.png)

1. **タイプ**&#x200B;の制約を追加します。

   ![](assets/clicks-predictive-content-add-constraint-hands.png)

1. スマートリストに必要なソースを選択します。

   ![](assets/pc-add-constraint.png)

1. 予測コンテンツにメールソースを使用する場合は、「**メール内リンクをクリック**」トリガーを追加します。メールを選択し、「**予測である**」制約（**true** と定義）を追加します。

   ![](assets/clicks-link-in-email-trigger-hands.png)

1. 必要に応じて、その他のフィルターを追加します。

   ![](assets/clicked-predictive-content-filter.png)

   >[!TIP]
   >
   >トリガーとフィルターの両方を含むスマートキャンペーンでは、トリガーが一番上に表示されます。トリガーされると、フィルター条件を満たす人のみがフローを通過します。

   >[!NOTE]
   >
   >複数のトリガーを使用する場合、いずれかのトリガーが有効化されると、フローに進みます。

   一連のリードに対してキャンペーンを同時に実行するには、[バッチスマートキャンペーンのスマートリストを定義する](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)方法を参照してください。

   >[!MORELIKETHIS]
   >
   >* [スマートキャンペーン用スマートリストの定義 | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md)
   >* [スマートキャンペーンへのフローステップの追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)
   >* [Web パーソナライゼーションアクティビティのスマートリストの定義](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/define-a-smart-list-for-web-personalization-activities.md)
   >* [Web リッチメディアの予測コンテンツを有効にする](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
   >* [コンテンツレコメンデーションバーを有効にする](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-the-content-recommendation-bar.md)

