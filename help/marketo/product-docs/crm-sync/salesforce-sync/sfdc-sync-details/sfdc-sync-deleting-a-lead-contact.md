---
unique-page-id: 7515131
description: SFDCの同期 — リード/連絡先の削除 — Marketto Docs — 製品ドキュメント
title: SFDCの同期 — リード/連絡先の削除
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# SFDC同期：リード/担当者の削除 {#sfdc-sync-deleting-a-lead-contact}

以下に、詳細を示します。

* Salesforceでリードが削除されたので、Marketorはユーザーを自動的に削除しません。 「SFDC Is Deleted」フラグがtrueに設定されている場合は、 必要に応じて、Marketorでこのフィールドをトリガーして削除できます。
* [「個人](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/delete-person.md) 」フロー・アクションの削除。 MKTO内の人物は削除されますが、削除する選択もでき `Salesforce` ます。

* [SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/delete-person-from-sfdc.md) Flow Action:これによりSFDCのリードは削除されますが、マーケティング担当者を削除することもできます。
* Salesforceでリードが削除された（ただし、その人がMarketorで削除されなかった）場合、その後、Salesforceと [同期](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) フローアクションを実行すると、Salesforceで新しいリードが作成されます。

つまり魔法のように動く！

![--](assets/image2015-5-20-15-3a3-3a27.png)

