---
unique-page-id: 557322
description: スマートリスト-Marketoドキュメント — 製品ドキュメントからの単一フローステップの実行
title: スマート・リストからの単一フロー・ステップの実行
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# スマートリストからの単一フローステップの実行{#run-a-single-flow-step-from-a-smart-list}

1回限りのフローステップを実行する場合は、スマートキャンペーン全体を作成する代わりに、スマートリスト内で1つのフローステップを使用できます。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/login-marketing-activities-1.png)

1. リストまたはスマートリストを選択し、**ユーザー**&#x200B;タブに移動します。

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >この機能は、静的なリストとスマートリストの両方にあります。

1. 「**すべて選択**」をクリックします。 **Ctrl/Cmd**&#x200B;を使用して、いくつかのレコードを手動でクリックして選択することもできます。

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >結果が複数のページにまたがる場合は、「**すべて選択**」をクリックすると、すべてのページのすべてのユーザーが選択されます。

1. 「**個人** **アクション**」で、選択したフローステップを選択します。 この例では、[データ値の変更](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)を使用します。

   ![](assets/personactions-hands.png)

1. **属性**&#x200B;を探して選択します。 この例では、州「California」を持つすべての人を「CA」に変更します。

   ![](assets/runaction-hands.png)

1. 新しい値を入力. 「**今すぐ実行**」をクリックします。

   ![](assets/runactionnewvalue-hands.png)

1. 多数のユーザーのデータ値を変更する場合は、数値を入力して変更の確認が必要になる場合があります。 「**Go For It**」をクリックします。

   ![](assets/changedatavalue.jpg)

すごい仕事！ 右上隅に単一フローステップのステータスが表示されます。

![](assets/completesingleflowaction.jpg)

完了したら、リストを更新すると、更新された情報が表示されます。
