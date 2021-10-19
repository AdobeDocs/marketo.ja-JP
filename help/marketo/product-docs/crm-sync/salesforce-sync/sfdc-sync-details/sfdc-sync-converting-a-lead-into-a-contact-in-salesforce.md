---
unique-page-id: 2953465
description: SFDC 同期 - Salesforce でリードを連絡先に変換 - Marketo ドキュメント - 製品ドキュメント
title: SFDC 同期 - Salesforce でリードを連絡先に変換
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '158'
ht-degree: 100%

---

# SFDC 同期：Salesforce でリードを連絡先に変換 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Salesforce で次の 3 つのシナリオを考えてみます（Marketo の[リードを変換フローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)は使用しません）。

1. リードを&#x200B;**新しい連絡先と新しいアカウント**&#x200B;に変換
1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**新しい連絡先**&#x200B;に変換

1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**既存連絡先**&#x200B;に変換（[マージ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md)と同じ）

3 つのケースはどれも、**Salesforce で 1 件の連絡先と 0 件のリード、Marketo で 1 件の連絡先と 0 件のリード**&#x200B;という結果になります。

Marketo では、レコードの SFDC タイプが連絡先になります。

>[!TIP]
>
>Salesforce で変換する場合は、[リードのカスタムフィールドが適切にマッピングされていること](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)を確認します。データは失いたくありません。

「変換済みのリード」および「リード変換済み」を使用して、トリガーおよびフィルタリングできます。
