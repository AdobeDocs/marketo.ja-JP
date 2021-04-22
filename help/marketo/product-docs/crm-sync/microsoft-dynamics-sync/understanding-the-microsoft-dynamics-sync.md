---
unique-page-id: 10098625
description: Microsoft Dynamics Sync -Marketoドキュメント — 製品ドキュメントについて
title: Microsoft Dynamicsの同期を理解しています
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 2%

---

# Microsoft Dynamics Syncを理解する{#understanding-the-microsoft-dynamics-sync}

MarketoとMicrosoft Dynamicsは連携しています。 販売とマーケティングのデータを同期させます。

>[!NOTE]
>
>Marketoでは、現時点でJava 7と互換性のあるSSL証明書のみがサポートされています。

## 同期の仕組み{#how-sync-works}

Marketoは毎日毎日、毎日毎日データをMicrosoft Dynamicsと同期します。 バックグラウンド同期をリアルタイムではなくバッチで使用します。

>[!NOTE]
>
>購読の最初の同期は、データベースのサイズに応じて、数分から数時間かかります。 Marketoは、データベース全体をDynamicsからコピーします。 その後、各同期は通常、変更されたデータのみを同期し、数秒または数分かかります。

Marketoとダイナミクスの同期は、リードとコンタクトの双方向です。 [Marketo]または[ダイナミクス]で変更を行うと、更新内容は両方のシステムに反映されます。 アカウントやオポチュニティなど、他のすべてのフィールドは、DynamicsからMarketoまで、一方向にのみ同期されます。

## MarketoとMicrosoft Dynamicsの間で同期されるもの{#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [連絡先](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsersのグループ）
* [商談](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

>[!NOTE]
>
>Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)用にMarketoに入力した[資格情報は、データの同期に使用されます。

>[!CAUTION]
>
>現在、Marketoダイナミクス同期のサンドボックス更新をサポートしていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketoサンドボックスが必要です。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。
