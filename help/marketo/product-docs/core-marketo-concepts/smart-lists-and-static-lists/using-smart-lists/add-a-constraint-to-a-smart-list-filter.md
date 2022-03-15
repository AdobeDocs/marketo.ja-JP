---
unique-page-id: 2949413
description: スマートリストフィルターへの制約の追加 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストフィルターへの制約の追加
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '175'
ht-degree: 100%

---

# スマートリストフィルターへの制約の追加 {#add-a-constraint-to-a-smart-list-filter}

スマートリストを作成する際に利用するフィルターの一部には、「制約」と呼ばれる高度なオプションが含まれています。制約を利用してフィルターやトリガーにさらなる条件を追加することで、検索をさらに絞り込むことができます。

以下に紹介する例では、「**[データ値変更済み](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)**」フィルターにいくつかの制約を追加して、リードステータスが MQL から SQL に変更されたリードを特定します。

>[!PREREQUISITES]
>
>* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
>* [スマートリストで「データ値変更済み」フィルターを使用します。](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md)
>


1. 「**マーケティング活動**」に移動します。

   ![](assets/ma-1.png)

1. 制約を追加するフィルターが設定されているスマートリストを選択して、「**スマートリスト**」タブをクリックします。

   ![](assets/two-3.png)

1. 「**制約を追加**」から「**前回の値**」を選択します。

   ![](assets/three-3.png)

1. 「**前回の値**」に入力します。この例では、「MQL」と入力します。

   ![](assets/four-2.png)

1. 「**制約を追加**」から「**新しい値**」を選択します。

   ![](assets/five.png)

1. 「**新しい値**」に入力します。この例では、「SQL」と入力します。

   ![](assets/six.png)

1. これで完了です。「**リード**」タブをクリックすると、過去 30 日間に「**ステータス**」が **MQL** から **SQL** に変わったすべての対象者が表示されます。
