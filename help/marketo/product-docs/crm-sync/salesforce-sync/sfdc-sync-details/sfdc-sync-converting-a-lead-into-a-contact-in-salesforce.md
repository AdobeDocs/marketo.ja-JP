---
unique-page-id: 2953465
description: SFDC 同期 - Salesforce でリードを取引先責任者に変換 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - Salesforce でリードを取引先責任者に変換
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 100%

---

# SFDC 同期：[!DNL Salesforce] でリードを取引先責任者に変換 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

[!DNL Salesforce] で次の 3 つのシナリオを考えてみます（Marketo の[リードを変換フローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)は使用しません）。

1. リードを&#x200B;**新しい連絡先と新しいアカウント**&#x200B;に変換
1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**新しい連絡先**&#x200B;に変換

1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**既存連絡先**&#x200B;に変換（[マージ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"}と同じ）

3 つのケースはどれも、**[!DNL Salesforce] で 1 件の取引先責任者と 0 件のリード、Marketo で 1 件の取引先責任者と 0 件の人物**&#x200B;という結果になります。

Marketo では、レコードの SFDC タイプが取引先責任者になります。

>[!TIP]
>
>[!DNL Salesforce] で変換する場合は、[リードのカスタムフィールドが適切にマッピングされていること](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)を確認します。データは失いたくありません。

「[!UICONTROL 変換済みのリード]」および「[!UICONTROL リード変換済み]」を使用して、トリガーおよびフィルタリングできます。
