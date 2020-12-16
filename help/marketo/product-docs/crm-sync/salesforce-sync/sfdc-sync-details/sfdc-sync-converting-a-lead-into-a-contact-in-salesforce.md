---
unique-page-id: 2953465
description: SFDC同期 — Salesforceの担当者へのリードの変換 — Marketto Docs — 製品ドキュメント
title: SFDC同期 — Salesforceでリードを連絡先に変換
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# SFDC同期：Salesforceでリードを連絡先に変換する {#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Salesforceの3つの異なるシナリオを考えてみましょう。(Marketoの「 [人物をコンバート」フローステップ](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) は使用しない)。

1. リードを **新しい連絡先と新しいアカウントに変換する**
1. リードを **既存のアカウントの****新しい連絡先に変換する**

1. リードを **既存のアカウントの** 既存の連絡先に変換する **(これは** 結合と同じように機能 [](sfdc-sync-merging-a-lead-contact-person.md))

3つすべての場合、Salesforceでは **1件の連絡先、1件の連絡先、およびMarketoでは1人の人がいない連絡先になります。**

Marketoでは、レコードにSFDC Type = Contactと表示されます。

>[!TIP]
>
>Salesforceでの変換時に、 [リードのカスタムフィールドが適切にマッピングされていることを確認します](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 データを失いたくない。

トリガーおよびフィルターには、次を使用できます。&quot;リードはコンバートされました&quot;と&quot;リードはコンバートされました。&quot;