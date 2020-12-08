---
unique-page-id: 2949413
description: スマートリストフィルタ追加ーに対する制約 — Marketto Docs — 製品ドキュメント
title: スマートリストフィルター追加の制約
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# スマートリストフィルター追加の制約 {#add-a-constraint-to-a-smart-list-filter}

スマートリストを作成する場合、一部のフィルターには*制約と呼ばれる高度なオプションがあります。 *これらは、フィルターやトリガーに追加して検索をさらに絞り込むための追加条件です。

この例では、「** [Data Value Changed](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**」フィルタに制約を追加して、MQLからSQLにステータスが変化したユーザーを検索します。

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**前提条件**
>
>* [スマートリストの作成](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [スマートリストでの「データ値の変更」フィルタの使用](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. 「 **マーケティングアクティビティ**」に移動します。

   ![](assets/ma-1.png)

1. 制約を追加するフィルタが含まれるスマートリストを選択し、[ **スマートリスト** ]タブをクリックします。

   ![](assets/two-3.png)

1. [ **追加拘束**]で、[ **前の値**]を選択します。

   ![](assets/three-3.png)

1. 「 **以前の値**」を入力します。 この例では、MQLを使用しています。

   ![](assets/four-2.png)

1. [ **追加拘束**]で、[ **新しい値**]を選択します。

   ![](assets/five.png)

1. 「 **新しい値**」を入力します。 この例では、SQLを使用しています。

   ![](assets/six.png)

1. うまくいった！ 「 **人物** 」タブをクリックして、 **ステータスが** MQL ******** SQLから過去30日間に変更されたすべての人物を表示します。

