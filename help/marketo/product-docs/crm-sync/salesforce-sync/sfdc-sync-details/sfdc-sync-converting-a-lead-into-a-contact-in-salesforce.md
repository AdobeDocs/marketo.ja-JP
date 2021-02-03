---
unique-page-id: 2953465
description: SFDC同期 — Salesforceの担当者へのリードの変換 — Marketto Docs — 製品ドキュメント
title: SFDC同期 — Salesforceでリードを連絡先に変換
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# SFDC同期：Salesforceのリードを連絡先に変換{#sfdc-sync-converting-a-lead-into-a-contact-in-salesforce}

Salesforceの3つの異なるシナリオを考えてみましょう。（Marketoでは、[人物をフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)に変換しない）

1. リードを&#x200B;**新しい連絡先と新しいアカウントに変換**
1. **既存のアカウント**&#x200B;の&#x200B;**新しい連絡先**&#x200B;にリードを変換する

1. **既存のアカウント**&#x200B;の&#x200B;**既存の連絡先**&#x200B;へのリードの変換（[結合](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-merging-a-lead-contact-person.md)と同じ）

3つの場合はすべて、**1件の連絡先、Salesforceでは1件のリード、Marketoでは1件の連絡先、Marketoでは1人の人がいないという結果になります。**

Marketoでは、レコードにSFDC Type = Contactと表示されます。

>[!TIP]
>
>Salesforceでの変換時に、[リードのカスタムフィールドが適切にマッピングされていることを確認してください](https://help.salesforce.com/apex/HTViewHelpDoc?id=customize_mapleads.htm)。 データを失いたくない。

次を使用して、トリガーとフィルターを行うことができます。&quot;リードはコンバートされました&quot;と&quot;リードはコンバートされました。&quot;
