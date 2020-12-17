---
unique-page-id: 2949413
description: スマートリストフィルタ追加ーに対する制約 — Marketto Docs — 製品ドキュメント
title: スマートリストフィルター追加の制約
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# スマ追加ートリストフィルターに対する制約{#add-a-constraint-to-a-smart-list-filter}

スマートリストを作成する場合、一部のフィルターには*制約と呼ばれる高度なオプションがあります。 *これらは、フィルターやトリガーに追加して検索をさらに絞り込むための追加条件です。

この例では、** [変更されたデータ値](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**フィルタに制約を追加して、MQLからSQLにステータスが変化した訪問者を検索します。

>[!PREREQUISITES]
>
>* [スマートリストの作成](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [スマートリストでの「データ値の変更」フィルタの使用](use-the-data-value-changed-filter-in-a-smart-list.md)

>



1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/ma-1.png)

1. 制約を追加するフィルターを持つスマートリストを選択し、「**スマートリスト**」タブをクリックします。

   ![](assets/two-3.png)

1. 「**追加制約**」で、「**以前の値**」を選択します。

   ![](assets/three-3.png)

1. **以前の値**&#x200B;を入力します。 この例では、MQLを使用しています。

   ![](assets/four-2.png)

1. 「**追加制約**」で、「**新しい値**」を選択します。

   ![](assets/five.png)

1. **新しい値**&#x200B;を入力します。 この例では、SQLを使用しています。

   ![](assets/six.png)

1. うまくいった！ 「**ユーザー**」タブをクリックすると、過去30日間に&#x200B;**ステータス**&#x200B;が&#x200B;**MQL**&#x200B;から&#x200B;**SQL**&#x200B;に変更されたすべてのユーザーが表示されます。

