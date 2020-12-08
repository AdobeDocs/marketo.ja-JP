---
unique-page-id: 10098625
description: Microsoft Dynamics Sync - Marketto Docs — 製品ドキュメントについて
title: Microsoft Dynamicsの同期を理解しています
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---


# Microsoft Dynamicsの同期を理解しています {#understanding-the-microsoft-dynamics-sync}

MarketorとMicrosoft Dynamicsは連携しています。 販売とマーケティングのデータを同期させます。

>[!NOTE]
>
>Marketorは、現時点ではJava 7と互換性のあるSSL証明書のみをサポートしています。

## 同期の仕組み {#how-sync-works}

Marketoは毎日毎日、データをMicrosoft Dynamicsと継続的に同期します。 バックグラウンド同期をリアルタイムではなくバッチで使用します。

>[!NOTE]
>
>購読の最初の同期は、データベースのサイズに応じて、数分から数時間かかります。 Marketorは、Dynamicsからデータベース全体をコピーします。 その後、各同期は通常、変更されたデータのみを同期し、数秒または数分かかります。

MarketoとDynamicsの同期は、リードと連絡先の双方向です。 MarketorまたはDynamicsで変更を行うと、両方のシステムに更新が反映されます。 アカウントやオポチュニティなど、他のすべてのフィールドは、DynamicsからMarketoへの1方向のみ同期されます。

## MarketoとMicrosoft Dynamicsの間で同期されるもの {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [連絡先](microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザー](microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsersのグループ）
* [オポチュニティ](microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Marketor for Dynamics [に入力した](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md) 資格情報は、データの同期に使用されます。

Dynamicsの同期には、多くのニュアンスと機能があります。 [ [Microsoft Dynamics同期の詳細]セクションの詳細を確認してください](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)。

>[!CAUTION]
>
>現在、Marketo Dynamics Syncのサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketo Sandboxが必要になります。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

>[!NOTE]
>
>**関連記事**
>
>* [同期設定](http://docs.marketo.com/display/docs/sync+setup)
   >
   >
* [Microsoft Dynamics同期の詳細](http://docs.marketo.com/display/docs/microsoft+dynamics+sync+details)

