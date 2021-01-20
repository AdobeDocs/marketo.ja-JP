---
unique-page-id: 1147034
description: SFDCキャンペーン追加- Marketto Docs — 製品ドキュメント
title: SFDC追加キャンペーン
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# SFDC追加キャンペーン{#add-to-sfdc-campaign}

>[!NOTE]
>
>Salesforceと統合されている場合にのみ使用できます。

## 概要{#overview}

このフローステップは、Marketorキャンペーンで使用することも、Salesforceキャンペーンでリードとして人を追加する単一のフローステップとして使用することもできます。 リードがSalesforceにまだ存在しない場合は、自動的に同期され、指定されたステータスでキャンペーンに追加されます。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用法{#usage}

1. リードを追加するSalesforceキャンペーンを探して選択します。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >キャンペーンリストにSalesforceキャンペーンが表示されない場合：
   >
   >  1. [キャンペーン同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)であることを確認します。
   >  1. [Marketo Sync User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)がSalesforceの[マーケティングユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md)であることを確認します。


   >[!TIP]
   >
   >Salesforceキャンペーン[マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)を使用すると、プログラムのクローン作成を簡単に行うことができます。

1. リードが追加されたときに、リードに割り当てるSalesforceキャンペーンメンバーのステータスを選択します。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >既にSalesforceキャンペーンのリードメンバーになっている人はスキップされ、そのステータスは更新されません。 代わりに、[SFDCキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md)のステータスを変更できます。
