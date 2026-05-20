---
unique-page-id: 2953465
description: Salesforceでリードを連絡先に変換した場合の処理について説明します。 Marketoでの変更内容の反映と、リードのコンバージョン済みトリガーとフィルターの使用について説明します。
title: SFDC 同期 - Salesforce でリードを取引先責任者に変換
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/Z5ApDpLvZhGu3-DeZHwQanilG1WILGFQF7VnDxQikr4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 169
ht-degree: 83%

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
>[!DNL Salesforce] で変換する場合は、[リードのカスタムフィールドが適切にマッピングされていること](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)を確認します。 データは失いたくありません。

「[!UICONTROL 変換済みのリード]」および「[!UICONTROL リード変換済み]」を使用して、トリガーおよびフィルタリングできます。
