---
unique-page-id: 2953465
description: SFDC Sync - Salesforce でのリードの連絡先への変換 – Marketoドキュメント – 製品ドキュメント
title: SFDC 同期 – Salesforce でのリードから連絡先への変換
exl-id: 9c9dbe9a-80a6-4153-ac86-96f85025fe77
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 57%

---

# SFDC 同期：Salesforce でリードを取引先責任者に変換 {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Salesforce における 3 つの異なるシナリオを想定してみてください：（Marketo Engageで [ ユーザーを変換フローステップ ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} を使用していない）

1. リードを&#x200B;**新しい連絡先と新しいアカウント**&#x200B;に変換
1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**新しい連絡先**&#x200B;に変換

1. リードを&#x200B;**既存アカウント**&#x200B;の&#x200B;**既存連絡先**&#x200B;に変換（[マージ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md){target="_blank"}と同じ）

3 つのケースはどれも、**Salesforce で 1 件の連絡先と 0 件のリード、Marketo で 1 件の連絡先と 0 件のリード**&#x200B;という結果になります。

Marketo では、レコードの SFDC タイプが連絡先になります。

>[!TIP]
>
>Salesforce で変換する場合は、[ リードカスタムフィールドが適切にマッピングされている ](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm){target="_blank"} ことを確認します。 データは失いたくありません。

「リードはコンバート済み」および「リードはコンバート済み」を使用してトリガーおよびフィルター処理できます。
