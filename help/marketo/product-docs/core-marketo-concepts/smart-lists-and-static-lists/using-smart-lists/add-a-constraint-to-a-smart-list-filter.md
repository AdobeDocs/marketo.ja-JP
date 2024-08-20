---
unique-page-id: 2949413
description: スマートリストフィルターへの制約の追加 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストフィルターへの制約の追加
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
source-git-commit: ac7d6b222ca561c88e0bf10aba7736c1b2eee3f7
workflow-type: ht
source-wordcount: '177'
ht-degree: 100%

---

# スマートリストフィルターへの制約の追加 {#add-a-constraint-to-a-smart-list-filter}

スマートリストを作成する際にフィルターの一部には、「制約」と呼ばれる高度なオプションが含まれています。制約を利用してフィルターやトリガーにさらなる条件を追加することで、検索をさらに絞り込むことができます。

以下に紹介する例では、「**[データ値変更済み](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}**」フィルターにいくつかの制約を追加して、リードステータスが MQL から SQL に変更されたリードを特定します。

>[!PREREQUISITES]
>
>* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [スマートリストで「データ値変更済み」フィルターを使用します。](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. 「**[!UICONTROL マーケティング活動]**」に移動します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. 制約を追加するフィルターが設定されているスマートリストを選択して、「**[!UICONTROL スマートリスト]**」タブをクリックします。

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. 「**[!UICONTROL 制約を追加]**」から「**[!UICONTROL 前回の値]**」を選択します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. 「**[!UICONTROL 前回の値]**」に入力します。この例では、MQL を使用します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. 「**[!UICONTROL 制約を追加]**」から「**[!UICONTROL 新しい値]**」を選択します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. 新しい値を入力します。この例では、SQL を使用します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. これで完了です。「**[!UICONTROL 人物]**」タブをクリックすると、過去 30 日間にステータスが「MQL」から「SQL」に変わったすべての対象者が表示されます。
