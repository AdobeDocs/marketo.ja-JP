---
unique-page-id: 1147034
description: SFDC キャンペーンに追加 - Marketo ドキュメント - 製品ドキュメント
title: SFDC キャンペーンに追加
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 88%

---

# SFDC キャンペーンに追加 {#add-to-sfdc-campaign}

>[!NOTE]
>
>Salesforce との連携時にのみ有効です。

## 概要 {#overview}

このフローステップを使用することで、Marketo のキャンペーン内、あるいは独立したフローステップから、Salesforce のキャンペーンにリードを追加することができます。リードがまだ Salesforce 内に存在していない場合、自動的に同期が行われ、指定されたステータスを付与してキャンペーンに追加されます。

![](assets/image2014-9-22-15-3a43-3a36.png)

## 使用方法 {#usage}

1. リードを追加したい Salesforce のキャンペーンを選択します。

   ![](assets/image2014-9-22-15-3a43-3a45.png)

   >[!TIP]
   >
   >キャンペーンリストに Salesforce キャンペーンが表示されない場合：
   >
   >  1. [キャンペーンの同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}になっていることを確認します。
   >  1. 次を確認します： [Marketo同期ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} is a [Marketing User](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"} Salesforce 内。

   >[!TIP]
   >
   >Salesforce のキャンペーンの[マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}を用いて指定すれば、プログラムを簡単に複製できます。

1. Salesforce のキャンペーンにリードが追加されたときに割り当てるメンバーステータスを選択します。

   ![](assets/image2014-9-22-15-3a45-3a2.png)

   >[!CAUTION]
   >
   >リードが既に Salesforce のキャンペーンのメンバーである場合、この処理は省略され、ステータスは更新されません。代わりに、[SFDC キャンペーン内のステータスの変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}を使用して、ステータスを変更できます。
