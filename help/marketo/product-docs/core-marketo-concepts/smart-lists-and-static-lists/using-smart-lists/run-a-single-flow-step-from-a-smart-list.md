---
unique-page-id: 557322
description: スマートリストからの単一フローステップの実行 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストからの単一フローステップの実行
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 100%

---

# スマートリストからの単一フローステップの実行 {#run-a-single-flow-step-from-a-smart-list}

1 回限りのフローステップを実行する場合は、スマートキャンペーン全体を作成する代わりに、スマートリスト内で 1 つのフローステップを使用できます。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 「**マーケティング活動**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. 人物を含むリストまたはスマートリストを選択し、「**人物**」タブをクリックします。

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >この機能は、静的リストとスマートリストの両方に用意されています。

1. 「**すべてを選択**」をクリックします。または、**Ctrl／Cmd** をクリックして、いくつかのレコードを手動で選択することもできます。

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >結果が複数のページにまたがる場合は、「**すべてを選択**」をクリックすると、すべてのページのすべての人物が選択されます。

1. 「**人物**」の「**アクション**」で選択したフローステップを選択します。この例では、「[データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)」を使用します。

   ![](assets/personactions-hands.png)

1. **属性**&#x200B;を検索して選択します。この例では、州「California」を持つすべての人物を対象に、州を「CA」に変更します。

   ![](assets/runaction-hands.png)

1. 新しい値を入力します。「**今すぐ実行**」をクリックします。

   ![](assets/runactionnewvalue-hands.png)

1. 多数の人物のデータ値を変更する場合は、その数を入力して変更を確定する必要がある場合があります。「**実行**」をクリックします。

   ![](assets/changedatavalue.jpg)

素晴らしいです。右上隅に単一フローステップのステータスが表示されます。

![](assets/completesingleflowaction.jpg)

完了後にリストを更新すると、更新された情報が表示されます。
