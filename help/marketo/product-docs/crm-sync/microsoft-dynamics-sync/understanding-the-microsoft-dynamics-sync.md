---
unique-page-id: 10098625
description: ' [!DNL Microsoft Dynamics]  同期について – Marketo ドキュメント – 製品ドキュメント'
title: Microsoft Dynamics 同期について
exl-id: bc87f744-7f1c-421b-8507-1a6e23d27fa2
feature: Microsoft Dynamics
source-git-commit: 0c0dd3355f979577ec194f9e8f935615515905c0
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 39%

---

# [!DNL Microsoft Dynamics] 同期について {#understanding-the-microsoft-dynamics-sync}

Marketoと [!DNL Microsoft Dynamics] は一緒だ。 お客様の販売データとマーケティングデータの同期を維持します。

>[!CAUTION]
>
>[!DNL Marketo Dynamics] 同期のサンドボックスの更新は、現在サポートされていません。 [!DNL Dynamics] CRM サンドボックスを更新する必要がある場合は、新しいMarketo サンドボックスが必要になります。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## 同期の仕組み {#how-sync-works}

Marketoは、毎日、継続的に [!DNL Microsoft Dynamics] とデータを同期します。 バックグラウンド同期が使用され、リアルタイムではなくバッチで行われます。

>[!NOTE]
>
>サブスクリプションの最初の同期には、データベースのサイズに応じて、数分から数時間かかります。Marketoは、[!DNL Dynamics] からデータベース全体をコピーします。 その後、各同期には、通常、数秒または数分かかり、変更されたデータのみが同期されます。

Marketoと [!DNL Dynamics] の同期は、リードと連絡先の双方向です。 Marketoまたは [!DNL Dynamics] のいずれかで変更を加えると、その変更は両方のシステムに反映されます。 アカウントやオポチュニティなどのその他のフィールドはすべて、[!DNL Dynamics] からMarketoに一方向にのみ同期されます。

## Marketoと [!DNL Microsoft Dynamics] の間で同期されるもの {#what-is-synced-between-marketo-and-microsoft-dynamics}

* [リード](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md)
* [取引先責任者](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md)
* [アカウント](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md)
* [ユーザー](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-user-sync.md)
* チーム（SystemUsers のグループ）
* [商談](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-opportunity-sync.md)
* [カスタムエンティティ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/enable-sync-for-a-custom-entity.md)

[Marketoに入力する資格情報  [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md) は、データの同期に使用されます。

>[!NOTE]
>
>ソースインスタンスが [!DNL Microsoft Dynamics] と統合されている場合、インスタンスのコピーはサポートされません。
