---
unique-page-id: 2949413
description: スマートリストフィルターに制約を追加する方法を説明します。 条件を追加してフィルターを絞り込み、リストを正確に表示します。
title: スマートリストフィルターへの制約の追加
exl-id: 5345019c-55e7-4afd-b583-90f1a687a71c
feature: Smart Lists
TQID: https://experienceleague.adobe.com/UqkPxJFs-78VaVMNgOa1p2sTuDo-FM74HXp3CAbruhA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 75%

---

# スマートリストフィルターへの制約の追加 {#add-a-constraint-to-a-smart-list-filter}

スマートリストを作成する際にフィルターの一部には、「制約」と呼ばれる高度なオプションが含まれています。 制約を利用してフィルターやトリガーにさらなる条件を追加することで、検索をさらに絞り込むことができます。

この例では、MQLからSQLにステータスが変更されたユーザーを検索するために、**[データ値が変更された](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}** フィルターに一部の制約を追加します。

>[!PREREQUISITES]
>
>* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [スマートリストで「データ値変更済み」フィルターを使用します。](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-the-data-value-changed-filter-in-a-smart-list.md){target="_blank"}

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-1.png)

1. 制約を追加するフィルターが設定されているスマートリストを選択して、「**[!UICONTROL スマートリスト]**」タブをクリックします。

   ![](assets/add-a-constraint-to-a-smart-list-filter-2.png)

1. 「**[!UICONTROL 制約を追加]**」から「**[!UICONTROL 前回の値]**」を選択します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-3.png)

1. 「**[!UICONTROL 前回の値]**」に入力します。 この例では、MQL を使用します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-4.png)

1. 「**[!UICONTROL 制約を追加]**」から「**[!UICONTROL 新しい値]**」を選択します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-5.png)

1. 新しい値を入力します。 この例では、SQL を使用します。

   ![](assets/add-a-constraint-to-a-smart-list-filter-6.png)

1. 「**[!UICONTROL 人物]**」タブをクリックすると、過去 30 日間にステータスが「MQL」から「SQL」に変わったすべての対象者が表示されます。
