---
unique-page-id: 4719283
description: Salesforce同期について —Marketoドキュメント — 製品ドキュメント
title: Salesforce同期について
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 2%

---

# Salesforce同期について{#understanding-the-salesforce-sync}

Marketoとセールスフォースは、ピースとニンジンのように一緒にいる。 販売とマーケティングのデータを同期させます。

## 同期の仕組み{#how-sync-works}

Marketoは毎日、セールスフォースと同期する。 各同期は、しばらく時間がかかり、その後5分間一時停止した後、開始が再び停止します。

>[!NOTE]
>
>購読での最初の同期は、MarketoがSalesforceからデータベース全体をコピーしているので、数時間から数日かかる場合があります。 その後、各同期は通常、変更されたデータのみを同期し、数秒または数分かかります。

![](assets/sync-illustration.png)

SalesforceとMarketoの同期は、リード、連絡先、Salesforceキャンペーンに対してのみ双方向です。 この場合、SalesforceまたはMarketoで変更を行うと、常に両方のシステムに更新が反映されます。 他の同期はすべてSalesforceからMarketoまでのみです。 各リンクの詳細については、以下のリンクをクリックしてください。

## MarketoとSalesforceの間で同期されるもの{#what-is-synced-between-marketo-and-salesforce}

* [リード](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-sync.md)
* [連絡先](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-lead-account-owner-sync.md)
* [商談](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-opportunity-sync.md)
* [Salesforceキャンペーン](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)
* [カスタムオブジェクト](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.md)
* [アクティビティ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-activity-sync.md)

>[!NOTE]
>
>Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)用にMarketoに入力した[資格情報は、データの同期に使用されます。 資格情報にアクセスできるデータのみが含まれます。

Marketoのセールスフォースとの同期は、世界で最も強力な存在です。 魔法のような感じ。変更が行われ、他のシステムが近日中に最新の状態になります。
