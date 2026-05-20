---
unique-page-id: 1147034
description: フローステップを使用してSalesforce キャンペーンにユーザーを追加する方法を説明します。 MarketoをSFDC キャンペーンに同期します。
title: SFDC キャンペーンに追加
exl-id: a5e14cc7-fd83-4a2c-aacb-e515669c9d21
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/7fp6JSlxwdg0Yoniw9E4VvmRNvyaVyhwyOc10veDvR4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 183
ht-degree: 80%

---

# SFDC キャンペーンに追加 {#add-to-sfdc-campaign}

Marketo Engage キャンペーンでこのフローステップを使用できます。または、単独のフローステップとして使用して、Salesforce キャンペーンで人物をリードとして追加できます。 リードがまだ Salesforce 内に存在していない場合、自動的に同期が行われ、指定されたステータスを付与してキャンペーンに追加されます。

>[!NOTE]
>
>[!DNL Salesforce] と統合されている場合にのみ使用できます。

![](assets/add-to-sfdc-campaign-1.png)

## 使用方法 {#usage}

1. リードを追加する [!DNL Salesforce] のキャンペーンを見つけて選択します。

   ![](assets/add-to-sfdc-campaign-2.png)

   >[!TIP]
   >
   >キャンペーンリストにSalesforce キャンペーンが表示されない場合：
   >
   > 1. [&#x200B; キャンペーン同期が有効になっていることを確認します](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}。
   > 1. [Marketo 同期ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}が、Salesforce で[マーケティングユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync/make-marketo-sync-user-a-marketing-user.md){target="_blank"}になっていることを確認します。

   >[!TIP]
   >
   >Salesforce のキャンペーンの[マイトークン](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}を用いて指定すれば、プログラムを簡単に複製できます。

1. [!DNL Salesforce] のキャンペーンにリードが追加されたときに割り当てるメンバーステータスを選択します。

   ![](assets/add-to-sfdc-campaign-3.png)

   >[!CAUTION]
   >
   >リードが既に Salesforce のキャンペーンのメンバーである場合、この処理は省略され、ステータスは更新されません。 代わりに、[SFDC キャンペーン内のステータスの変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-status-in-sfdc-campaign.md){target="_blank"}を使用して、ステータスを変更できます。
