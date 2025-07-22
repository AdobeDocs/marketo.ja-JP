---
unique-page-id: 4719283
description: Salesforce 同期について — Marketo ドキュメント — 製品ドキュメント
title: Salesforce 同期について
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 57%

---

# [!DNL Salesforce] 同期について {#understanding-the-salesforce-sync}

Marketo Engageと Salesforce は密接に連携しています。お客様の販売データとマーケティングデータの同期を維持します。

## 同期の仕組み {#how-sync-works}

Marketoは毎日、[!DNL Salesforce] と同期します。 各同期は、しばらく時間がかかり、5 分間一時停止してから、再び開始します。

>[!NOTE]
>
>Marketoが [!DNL Salesforce] からデータベース全体をコピーするので、サブスクリプションの最初の同期には数時間または数日かかる場合があります。 その後、各同期には、通常、数秒または数分かかり、変更されたデータのみが同期されます。

![](assets/sync-illustration.png)

[!DNL Salesforce] とMarketoの同期は、リード、連絡先および [!DNL Salesforce] キャンペーンに対してのみ双方向です。 このような場合、[!DNL Salesforce] またはMarketoで変更を加えるたびに、その変更が両方のシステムに反映されます。 その他の同期はすべて [!DNL Salesforce] からMarketoへの同期のみです。 詳しくは、次のリンクをクリックしてください。

## Marketoと [!DNL Salesforce] の間で同期されるもの {#what-is-synced-between-marketo-and-salesforce}

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
>[Salesforce 用に Marketo で入力した資格情報](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}は、データの同期に使用されます。その資格情報でアクセスできるデータのみが含まれます。

Marketoと [!DNL Salesforce] のシンクロは、世界で最もパワフルなものです。 まるで魔法のように、変更を加えるとすぐに他のシステムが最新の状態になります。
