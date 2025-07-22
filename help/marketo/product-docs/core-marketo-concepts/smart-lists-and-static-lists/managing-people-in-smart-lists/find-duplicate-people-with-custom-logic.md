---
unique-page-id: 2952636
description: カスタムロジックでの重複リードの検索 - Marketo ドキュメント - 製品ドキュメント
title: カスタムロジックでの重複リードの検索
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 63%

---

# カスタムロジックでの重複リードの検索 {#find-duplicate-people-with-custom-logic}

Marketo Engageには、メールアドレスを照合して重複するユーザーを検索するシステムスマートリストがあります。 別のフィールドを使用して重複を検索する方法を次に示します。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. 「**[!UICONTROL マーケティング活動]**」領域に移動します。

![](assets/ma-2.png)

1. スマート・リストを選択し、「**[!UICONTROL スマート・リスト]**」タブをクリックします。

   ![](assets/two-4.png)

1. **[!UICONTROL 重複フィールド]**&#x200B;フィルターを探してキャンバスにドラッグします。

   ![](assets/three-4.png)

1. 次の 4 つのオプションの中から 1 つを選択します。

   * [!UICONTROL &#x200B; メールアドレス &#x200B;]
   * [!UICONTROL &#x200B; 姓名 &#x200B;]
   * [!UICONTROL &#x200B; 姓 &#x200B;]
   * [!UICONTROL &#x200B; 更新日時 &#x200B;]

   >[!NOTE]
   >
   >「メールアドレス」を除くすべてのフィールドでは、大文字と小文字が区別されます。したがって、「姓名」フィールドに「john doe」と入力すると、「John Doe」は結果に&#x200B;_返されません_。

   ![](assets/four-2.png)

   完了です。スマートリストを実行して、以前に選択したフィールドで同じ値を持つ人物を検索します。
