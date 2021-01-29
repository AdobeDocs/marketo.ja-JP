---
unique-page-id: 10098625
description: Microsoft Dynamics Sync - Marketto Docs — 製品ドキュメントについて
title: Microsoft Dynamicsの同期を理解しています
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---


# Microsoft Dynamics Syncを理解する{#understanding-the-microsoft-dynamics-sync}

MarketorとMicrosoft Dynamicsは連携しています。 販売とマーケティングのデータを同期させます。

>[!NOTE]
>
>Marketorは、現時点ではJava 7と互換性のあるSSL証明書のみをサポートしています。

## 同期の仕組み{#how-sync-works}

Marketoは毎日毎日、データをMicrosoft Dynamicsと継続的に同期します。 バックグラウンド同期をリアルタイムではなくバッチで使用します。

>[!NOTE]
>
>購読の最初の同期は、データベースのサイズに応じて、数分から数時間かかります。 Marketorは、Dynamicsからデータベース全体をコピーします。 その後、各同期は通常、変更されたデータのみを同期し、数秒または数分かかります。

MarketoとDynamicsの同期は、リードと連絡先の双方向です。 MarketorまたはDynamicsで変更を行うと、両方のシステムに更新が反映されます。 アカウントやオポチュニティなど、他のすべてのフィールドは、DynamicsからMarketoへの1方向のみ同期されます。

## MarketoとMicrosoft Dynamicsの間で同期されるもの{#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [連絡先](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsersのグループ）
* [オポチュニティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Marketor for Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)に入力した[資格情報は、データの同期に使用されます。

>[!CAUTION]
>
>現在、Marketo Dynamics Syncのサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketo Sandboxが必要になります。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。
