---
unique-page-id: 4719283
description: Salesforce 同期について — Marketo ドキュメント — 製品ドキュメント
title: Salesforce 同期について
exl-id: 658c81ff-5fb3-4ad8-8759-da55bbf4e263
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '219'
ht-degree: 100%

---

# Salesforce 同期について {#understanding-the-salesforce-sync}

Marketo と Salesforce は、非常に相性がよく、お客様の販売データとマーケティングデータの同期を維持します。

## 同期の仕組み {#how-sync-works}

Marketo は、毎日、常に Salesforce と同期します。各同期は、しばらく時間がかかり、5 分間一時停止してから、再び開始します。

>[!NOTE]
>
>Marketo が Salesforce からデータベース全体をコピーするので、サブスクリプションの最初の同期には、数時間または数日かかる場合があります。その後、各同期には、通常、数秒または数分かかり、変更されたデータのみが同期されます。

![](assets/sync-illustration.png)

Salesforce と Marketo の間の同期は、リード、連絡先、Salesforce キャンペーンのみ双方向です。この場合、Salesforce または Marketo で変更を加えるたびに、更新内容が両方のシステムに反映されます。その他のすべての同期は、Salesforce から Marketo に対してのみです。詳しくは、次のリンクをクリックしてください。

## Marketo と Salesforce の間で同期されるもの {#what-is-synced-between-marketo-and-salesforce}

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
>[Salesforce 用に Marketo で入力した認証情報](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)は、データの同期に使用されます。その認証情報でアクセスできるデータのみが含まれます。

Marketo と Salesforce の同期は、世界で最も強力です。まるで魔法のように、変更を加えるとすぐに他のシステムが最新の状態になります。
