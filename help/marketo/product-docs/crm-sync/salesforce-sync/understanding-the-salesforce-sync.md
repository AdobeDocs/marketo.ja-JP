---
unique-page-id: 4719283
description: Salesforce同期について — Marketto Docs — 製品ドキュメント
title: Salesforce同期について
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Salesforce同期について{#understanding-the-salesforce-sync}

MarketoとSalesforceは、ピースとニンジンのように連携しています。 販売とマーケティングのデータを同期させます。

## 同期の仕組み{#how-sync-works}

マーケティング担当者は、毎日、Salesforceと同期します。 各同期は、しばらく時間がかかり、その後5分間一時停止した後、開始が再び停止します。

>[!NOTE]
>
>購読での最初の同期は、MarketoがSalesforceからデータベース全体をコピーするので、数時間か数日かかる場合があります。 その後、各同期は通常、変更されたデータのみを同期し、数秒または数分かかります。

![](assets/sync-illustration.png)

SalesforceとMarketoの同期は、リード、連絡先、Salesforceのキャンペーンに対してのみ双方向です。 この場合、SalesforceまたはMarketoで変更を行うと、常に両方のシステムに更新が反映されます。 他のすべての同期は、SalesforceからMarketoへのみ行われます。 各リンクの詳細については、以下のリンクをクリックしてください。

## MarketoとSalesforceの間で同期されるもの{#what-is-synced-between-marketo-and-salesforce}

* [リード](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [連絡先](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [オポチュニティ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforceキャンペーン](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [カスタムオブジェクト](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [アクティビティ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Marketo for Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)に入力する[資格情報は、データの同期に使用されます。 資格情報にアクセスできるデータのみが含まれます。

マーケットとSalesforceの同期は、世界で最も強力なソリューションです。 魔法のような感じ。変更が行われ、他のシステムが近日中に最新の状態になります。
