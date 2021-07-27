---
unique-page-id: 10098625
description: Microsoft Dynamics Syncについて — Marketoドキュメント — 製品ドキュメント
title: Microsoft Dynamics同期について
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 80651a7d3d416f27ef13184b11757943c98bd781
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%

---

# Microsoft Dynamics同期について {#understanding-the-microsoft-dynamics-sync}

MarketoとMicrosoft Dynamicsは連携します。 お客様の販売データとマーケティングデータを同期させます。

>[!NOTE]
>
>Marketoでは、現時点でJava 7と互換性のあるSSL証明書のみをサポートしています。

>[!CAUTION]
>
>現在、Marketo Dynamics Syncのサンドボックス更新はサポートされていません。 Dynamics CRMサンドボックスを更新する必要がある場合は、新しいMarketoサンドボックスが必要です。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## 同期の仕組み {#how-sync-works}

Marketoは、毎日、毎日、Microsoft Dynamicsとデータを継続的に同期します。 リアルタイムではなく、バックグラウンド同期を使用してバッチで実行します。

>[!NOTE]
>
>サブスクリプションの最初の同期は、データベースのサイズに応じて、数分から数時間かかります。 Marketoは、Dynamicsからデータベース全体をコピーします。 その後、各同期には通常、数秒または数分かかり、変更されたデータのみが同期されます。

MarketoとDynamicsの間の同期は、リードとコンタクトに対して双方向です。 MarketoまたはDynamicsで変更を加えると、更新内容は両方のシステムに反映されます。 アカウントやオポチュニティなど、その他すべてのフィールドは、DynamicsからMarketoへの1つの方法でのみ同期されます。

## MarketoとMicrosoft Dynamicsの間で同期されるもの {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [連絡先](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsersのグループ）
* [商談](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-custom-entity-sync.md)

Marketo for Dynamicsに入力した[資格情報は、データの同期に使用されます。](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)

>[!NOTE]
>
>ソースインスタンスがMicrosoft Dynamicsと統合されている場合、インスタンスコピーはサポートされません。
