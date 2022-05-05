---
description: Veeva CRM 同期について — Marketoドキュメント — 製品ドキュメント
title: Veeva CRM 同期について
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
source-git-commit: 884c9a27f3876ec3036f2f7187db30565cdd49a7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 8%

---

# Veeva CRM 同期について {#understanding-the-veeva-crm-sync}

いくつかの簡単な手順で、Adobe Marketo Engageと Veeva CRM 間の同期を簡単に実行できます。

## 同期の仕組み {#how-the-sync-works}

Marketo Engageは毎日 Veeva CRM と同期します。 各同期には時間がかかり、5 分間一時停止した後、再び開始します。

>[!NOTE]
>
>最初の同期には、Marketo Engageが Veeva からデータベース全体をコピーするので、数時間から数日かかる場合があります。 その後、各同期には通常数分（秒）かかり、変更されたデータのみが同期されます。

![](assets/understanding-the-veeva-sync-1.png)

Veeva とMarketo Engageの同期は、担当者アカウントオブジェクトの連絡先フィールドに対してのみ双方向です。 この場合、Veeva またはMarketo Engageで変更を加えると、常に両方のシステムで更新が反映されます。 その他の同期はすべて Veeva からMarketo Engageのみです。 詳しくは、次のリンクをクリックしてください。

## Marketo Engageと Veeva 間の同期内容 {#what-is-synced-between-marketo-engage-and-veeva}

* [担当者アカウント](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target=&quot;_blank&quot;}
* ユーザー
* [呼び出しおよび呼び出しキーオブジェクト](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
* [カスタムオブジェクト](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}

## 留意事項 {#things-to-know}

* この [Veeva のMarketo Engageで入力した資格情報](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target=&quot;_blank&quot;} は、データの同期に使用されます。 その認証情報でアクセスできるデータのみが含まれます。

* Veeva CRM は force.com に基づいており、プラットフォームとのリッチエクスペリエンスMarketo Engageがこの同期に継承されます。

* Veeva CRM には次の内容が表示されます。リード、連絡先、アカウント（ビジネスアカウント、商談、キャンペーン、アクティビティ） ただし、Marketo Engageとの同期ではサポートされていません。
