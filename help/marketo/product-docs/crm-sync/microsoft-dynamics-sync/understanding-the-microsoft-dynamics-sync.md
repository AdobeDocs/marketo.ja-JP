---
unique-page-id: 10098625
description: Microsoft Dynamics同期によってMarketoと Dynamics のデータの同期を維持する方法について説明します。 リードおよび連絡先に対する同期対象と双方向同期の仕組みを確認します。
title: Microsoft Dynamics 同期について
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 88%

---

# [!DNL Microsoft Dynamics] 同期について {#understanding-the-microsoft-dynamics-sync}

Marketo と [!DNL Microsoft Dynamics] は連携します。お客様の販売データとマーケティングデータの同期を維持します。

>[!CAUTION]
>
>現在、[!DNL Marketo Dynamics] 同期のサンドボックス更新はサポートされていません。[!DNL Dynamics] CRM サンドボックスを更新する必要がある場合は、新しい Marketo サンドボックスが必要です。詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## 同期の仕組み {#how-sync-works}

Marketo は、毎日、常に [!DNL Microsoft Dynamics] と継続的にデータを同期します。バックグラウンド同期が使用され、リアルタイムではなくバッチで行われます。

>[!NOTE]
>
>サブスクリプションの最初の同期には、データベースのサイズに応じて、数分から数時間かかります。Marketo は、[!DNL Dynamics] からデータベース全体をコピーします。その後、各同期には、通常、数秒または数分かかり、変更されたデータのみが同期されます。

Marketo と [!DNL Dynamics] の間の同期は、リードと取引先責任者が双方向です。Marketo または [!DNL Dynamics] で変更を加えると、更新内容が両方のシステムに反映されます。その他のすべてのフィールド（アカウントや商談など）は、[!DNL Dynamics] から Marketo への一方行でのみ同期されます。

## Marketo と [!DNL Microsoft Dynamics] の間で同期されるもの {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [取引先責任者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsers のグループ）
* [商談](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

[ [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) 用に Marketo で入力した資格情報は、データの同期に使用されます。

>[!NOTE]
>
>ソースインスタンスが [!DNL Microsoft Dynamics] と統合されている場合、インスタンスコピーはサポートされません。
