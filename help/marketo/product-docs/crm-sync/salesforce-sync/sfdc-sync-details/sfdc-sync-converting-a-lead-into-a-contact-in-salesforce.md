---
unique-page-id: 2953465
description: SFDC Sync - Salesforceでのリードの連絡先への変換 – Marketo ドキュメント – 製品ドキュメント
title: SFDC同期 – Salesforceでのリードの連絡先への変換
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 37%

---

# SFDC Sync:[!DNL Salesforce] でのリードから連絡先への変換 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

[!DNL Salesforce] では、（Marketoの [ ユーザーを変換フローステップ ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) を使用しない） 3 つの異なるシナリオを想定してみてください

1. リードを&#x200B;**新しい連絡先と新しいアカウント**&#x200B;に変換
1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**新しい連絡先**&#x200B;に変換

1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**既存連絡先**&#x200B;に変換（[マージ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"}と同じ）

3 つのケースでは、最終的に **1 に連絡し、[!DNL Salesforce] と 1 にはリードがなく、Marketoには人物がいません。**

Marketo では、レコードの SFDC タイプが連絡先になります。

>[!TIP]
>
>[!DNL Salesforce] で変換する場合は、[ リードカスタムフィールドが適切にマッピングされている ](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm) ことを確認します。 データは失いたくありません。

「[!UICONTROL &#x200B; リードはコンバート済み &#x200B;]」および「[!UICONTROL &#x200B; リードはコンバート済み &#x200B;]」を使用してトリガーおよびフィルター処理できます。
