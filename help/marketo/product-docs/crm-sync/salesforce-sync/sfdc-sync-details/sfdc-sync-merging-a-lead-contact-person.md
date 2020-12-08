---
unique-page-id: 7515133
description: SFDC同期 — リード/連絡先/担当者の結合 — マーケティング担当者ドキュメント — 製品ドキュメント
title: SFDC同期 — リード/連絡先/担当者の結合
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# SFDC同期：リード/連絡先/個人のマージ {#sfdc-sync-merging-a-lead-contact-person}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

ルールをリストするだけで良い場合もあります。 次に進みます。

* Salesforce ****&#x200B;で2つのリードを結合する場合、通常の同期はMarketoに指示し、リードはMarketoのユーザーとして自動的に結合されます。
* 2人の人を **Marketo** Suiteに結合すると、Salesforceのリードと同じプロセスが実際に呼び出されます。 引き続き自動的に機能します。
* リー **ド（人）を連絡先にマージするのも** 、同じように機能します。 両側に1つの接触が生じます。
* 結合時に、デフォルトのスコアが合計されます。

>[!NOTE]
>
>**例**
>
>3つのリード（人）をそれぞれ10のスコアで結合すると、1つのリード（人）とスコア30の結果になります。

* 競合するフィールド値が「勝者レコード」から取得されます。 （レコード=結果のリードまたは連絡先）
* 「失われたレコード」（非表示になっているレコード）に値が指定され、勝者レコードがない場合、失われたレコードは保持されます。 言い換えると、「値がないよりも値が良い」という意味です。
* すべてのアクティビティログ項目がマージされます。

>[!NOTE]
>
>**ディープダイブ**
>
>Deep diveを参照してください [](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)。

