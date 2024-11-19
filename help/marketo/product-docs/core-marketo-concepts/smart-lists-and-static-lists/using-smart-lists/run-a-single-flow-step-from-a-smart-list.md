---
unique-page-id: 557322
description: スマートリストからの単一フローステップの実行 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストからの単一フローステップの実行
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: e0106eddf3ed6ecd2d9d90147a56258f61958665
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 72%

---

# スマートリストからの単一フローステップの実行 {#run-a-single-flow-step-from-a-smart-list}

1 回限りのフローステップを実行する場合は、スマートキャンペーン全体を作成する代わりに、スマートリスト内で 1 つのフローステップを使用できます。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. 「**[!UICONTROL マーケティング活動]**」に移動します。

   ![](assets/run-a-single-flow-step-from-a-smart-list-1.png)

1. ユーザーが含まれているリストまたはスマートリストを選択し、「**[!UICONTROL ユーザー]**」タブに移動します。

   ![](assets/run-a-single-flow-step-from-a-smart-list-2.png)

   >[!TIP]
   >
   >静的リストとスマート・リストの両方にこの機能があります。

1. 「**[!UICONTROL すべてを選択]**」をクリックします。または、**Ctrl／Cmd** をクリックして、いくつかのレコードを手動で選択することもできます。

   ![](assets/run-a-single-flow-step-from-a-smart-list-3.png)

   >[!NOTE]
   >
   >結果が複数のページにまたがる場合は、「**[!UICONTROL すべてを選択]**」をクリックすると、すべてのページのすべての人物が選択されます。

1. **[!UICONTROL 人物アクション]** で、目的のフローステップを選択します。 この例では、「[データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}」を使用します。

   ![](assets/run-a-single-flow-step-from-a-smart-list-4.png)

1. **[!UICONTROL 属性]**&#x200B;を検索して選択します。この例では、州「California」を持つすべての人物を対象に、州を「CA」に変更します。

   ![](assets/run-a-single-flow-step-from-a-smart-list-5.png)

1. 新しい値を入力します。「**[!UICONTROL 今すぐ実行]**」をクリックします。

   ![](assets/run-a-single-flow-step-from-a-smart-list-6.png)

1. 多数の人物のデータ値を変更する場合は、その数を入力して変更を確定する必要がある場合があります。「**[!UICONTROL 実行]**」をクリックします。

   ![](assets/run-a-single-flow-step-from-a-smart-list-7.png)

素晴らしいです。右上隅に単一フローステップのステータスが表示されます。

![](assets/run-a-single-flow-step-from-a-smart-list-8.png)

完了後にリストを更新すると、更新された情報が表示されます。
