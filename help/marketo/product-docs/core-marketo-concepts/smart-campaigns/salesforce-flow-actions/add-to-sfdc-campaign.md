---
unique-page-id: 1147034
description: SFDC キャンペーンに追加 - Marketo ドキュメント - 製品ドキュメント
title: SFDC キャンペーンに追加
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 100%

---

# SFDC キャンペーンに追加 {#add-to-sfdc-campaign}

Marketo Engage キャンペーンでこのフローステップを使用できます。または、単独のフローステップとして使用して、Salesforce キャンペーンで人物をリードとして追加できます。リードがまだ Salesforce 内に存在していない場合、自動的に同期が行われ、指定されたステータスを付与してキャンペーンに追加されます。

>[!NOTE]
>
>[!DNL Salesforce] と統合されている場合にのみ使用できます。

![](assets/add-to-sfdc-campaign-1.png)

## 使用方法 {#usage}

1. リードを追加する [!DNL Salesforce] のキャンペーンを見つけて選択します。

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >キャンペーンリストに Salesforce のキャンペーンが表示されない場合は、次を確認してください。
   >
   > 1. [キャンペーンの同期が有効](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}になっていることを確認します。
   > 1. [Marketo 同期ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}が、Salesforce で[マーケティングユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}になっていることを確認します。

   >[!TIP]
   >
   >Salesforce のキャンペーンの[マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}を用いて指定すれば、プログラムを簡単に複製できます。

1. [!DNL Salesforce] のキャンペーンにリードが追加されたときに割り当てるメンバーステータスを選択します。

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >リードが既に Salesforce のキャンペーンのメンバーである場合、この処理は省略され、ステータスは更新されません。代わりに、[SFDC キャンペーン内のステータスの変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}を使用して、ステータスを変更できます。
