---
unique-page-id: 10098625
description: Microsoft Dynamics 同期について - Marketo ドキュメント - 製品ドキュメント
title: Microsoft Dynamics 同期について
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
source-git-commit: 297ff02ba2c1173cabfecdef283e97c87c922480
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 100%

---

# Microsoft Dynamics 同期について {#understanding-the-microsoft-dynamics-sync}

Marketo と Microsoft Dynamics は適切に連携して、お客様の販売データとマーケティングデータの同期を維持します。

>[!NOTE]
>
>Marketo は、現時点では、Java 7  と互換性のある SSL 証明書のみをサポートしています。

>[!CAUTION]
>
>現在、Marketo Dynamics Sync のサンドボックス更新はサポートされていません。Dynamics CRM サンドボックスを更新する必要がある場合は、新しい Marketo サンドボックスが必要です。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## 同期の仕組み {#how-sync-works}

Marketo は、毎日、1 日中、Microsoft Dynamics と継続的にデータを同期します。バックグラウンド同期が使用され、リアルタイムではなくバッチで行われます。

>[!NOTE]
>
>サブスクリプションの最初の同期には、データベースのサイズに応じて、数分から数時間かかります。Marketo は、Dynamics からデータベース全体をコピーします。その後、各同期には、通常、数秒または数分かかり、変更されたデータのみが同期されます。

Marketo と Dynamics の間の同期は、リードと連絡先が双方向です。Marketo または Dynamics で変更を加えると、更新内容が両方のシステムに反映されます。その他のすべてのフィールド（アカウントや商談など）は、Dynamics から Marketo への一方行でのみ同期されます。

## Marketo と Microsoft Dynamics の間で同期されるもの {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [連絡先](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsers のグループ）
* [商談](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

[Dynamics 用に Marketo で入力した認証情報](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)は、データの同期に使用されます。

>[!NOTE]
>
>ソースインスタンスが Microsoft Dynamics と統合されている場合、インスタンスコピーはサポートされません。
