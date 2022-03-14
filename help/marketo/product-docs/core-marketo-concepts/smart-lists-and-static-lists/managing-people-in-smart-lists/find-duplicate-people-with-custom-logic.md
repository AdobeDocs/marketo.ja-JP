---
unique-page-id: 2952636
description: カスタムロジックでの重複リードの検索 - Marketo ドキュメント - 製品ドキュメント
title: カスタムロジックでの重複リードの検索
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '137'
ht-degree: 100%

---

# カスタムロジックでの重複リードの検索 {#find-duplicate-people-with-custom-logic}

Marketo には、メールアドレスを照合して重複するリードを見つけるシステムスマートリストがあります。別のフィールドを使用して重複を検索する方法を次に示します。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. 「**マーケティング活動**」領域に移動します。

![](assets/ma-2.png)

1. スマートリストを選択し、「**スマートリスト**」タブをクリックします。

   ![](assets/two-4.png)

1. **重複フィールド**&#x200B;フィルターを探してキャンバスにドラッグします。

   ![](assets/three-4.png)

1. 次の 4 つのオプションの中から 1 つを選択します。

   * メールアドレス
   * 氏名
   * 姓
   * 更新時刻

   >[!NOTE]
   >
   >「メールアドレス」を除くすべてのフィールドでは、大文字と小文字が区別されます。したがって、「姓名」フィールドに「john doe」と入力すると、「John Doe」は結果に&#x200B;_返されません_。

   ![](assets/four-2.png)

   完了です。スマートリストを実行すると、あらかじめ選択したフィールドに同じ値を持つリードを検索できます。
