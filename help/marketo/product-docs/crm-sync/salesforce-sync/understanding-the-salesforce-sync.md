---
unique-page-id: 4719283
description: Salesforceの同期でMarketoとSalesforceのデータを同期する方法について説明します。 同期の仕組みと、リードと連絡先の双方向同期の仕組みをご覧ください。
title: Salesforce 同期について
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/1H8ol0eKIzfQoQR-Je4jCdZX7R-rWWD63qrhkrsWtyg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 224
ht-degree: 81%

---

# [!DNL Salesforce] 同期について {#understanding-the-salesforce-sync}

Salesforceの同期でMarketoとSalesforceのデータを同期する方法について説明します。

## 同期の仕組み {#how-sync-works}

Marketo は、毎日、常に [!DNL Salesforce] と同期します。 各同期は、しばらく時間がかかり、5 分間一時停止してから、再び開始します。

>[!NOTE]
>
>Marketo が [!DNL Salesforce] からデータベース全体をコピーするので、サブスクリプションの最初の同期には、数時間または数日かかる場合があります。 その後、各同期には、通常、数秒または数分かかり、変更されたデータのみが同期されます。

![](assets/sync-illustration.png)

[!DNL Salesforce] と Marketo の間の同期は、リード、取引先責任者、[!DNL Salesforce] キャンペーンのみ双方向です。 この場合、[!DNL Salesforce] または Marketo で変更を加えるたびに、更新内容が両方のシステムに反映されます。 その他のすべての同期は、[!DNL Salesforce] から Marketo に対してのみです。 詳しくは、次のリンクをクリックしてください。

## Marketo と [!DNL Salesforce] の間で同期されるもの {#what-is-synced-between-marketo-and-salesforce}

* [リード](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md){target="_blank"}
* [取引先責任者](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"}
* [アカウント](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"}
* [ユーザ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md){target="_blank"}
* [商談](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md){target="_blank"}
* [Salesforce キャンペーン](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
* [カスタムオブジェクト](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md){target="_blank"}
* [アクティビティ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md){target="_blank"}

>[!NOTE]
>
>[Salesforce 用に Marketo で入力した資格情報](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}は、データの同期に使用されます。 その資格情報でアクセスできるデータのみが含まれます。

Marketo と [!DNL Salesforce] の同期は、世界で最も強力です。 まるで魔法のように、変更を加えるとすぐに他のシステムが最新の状態になります。
