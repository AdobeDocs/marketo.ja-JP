---
unique-page-id: 7515133
description: SFDC同期 — リード/連絡先/担当者の結合 — マーケティング担当者ドキュメント — 製品ドキュメント
title: SFDC同期 — リード/連絡先/担当者の結合
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# SFDC同期：リード/連絡先/人物のマージ{#sfdc-sync-merging-a-lead-contact-person}

ルールをリストするだけで良い場合もあります。 次に進みます。

* **Salesforce**&#x200B;で2つのリードを結合すると、通常の同期はMarketoに指示し、リードはMarketoの担当者として自動的に結合されます。
* **Marketo**&#x200B;に2人を結合すると、Salesforceのリードと同じプロセスが実際に呼び出されます。 引き続き自動的に機能します。
* **リード（人）をコンタクト**&#x200B;に結合するのも同じように動きます。 両側に1つの接触が生じます。
* 結合時に、デフォルトのスコアが合計されます。

>[!NOTE]
>
>3つのリード（人）をそれぞれ10のスコアで結合すると、1つのリード（人）とスコア30の結果になります。

* 競合するフィールド値が「勝者レコード」から取得されます。 （レコード=結果のリードまたは連絡先）
* 「失われたレコード」（非表示になっているレコード）に値が指定され、勝者レコードがない場合、失われたレコードは保持されます。 言い換えると、「値がないよりも値が良い」という意味です。
* すべてのアクティビティログ項目がマージされます。

>[!NOTE]
>
>[マーケットの人々を結合する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)について詳しくは、ディープダイブを参照してください。
