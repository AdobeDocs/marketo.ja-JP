---
unique-page-id: 2952636
description: カスタムロジックを使用して重複するユーザーを見つける方法を説明します。 スマートリストを作成し、基準ごとに重複を識別できます。
title: カスタムロジックでの重複リードの検索
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
TQID: https://experienceleague.adobe.com/-NvWt-eEzngL0QY7Kyl6lfjd75WcoQmcq3IiN7Uc6-w
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 149
ht-degree: 77%

---

# カスタムロジックでの重複リードの検索 {#find-duplicate-people-with-custom-logic}

Marketo Engage には、メールアドレスを照合して重複するリードを見つけるシステムスマートリストがあります。 別のフィールドを使用して、との重複を見つける場合は、次の手順に従います。

>[!PREREQUISITES]
>
>[スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. 「**[!UICONTROL マーケティング活動]**」領域に移動します。

![](assets/ma-2.png)

1. スマートリストを選択し、「**[!UICONTROL スマートリスト]**」タブをクリックします。

   ![](assets/two-4.png)

1. **[!UICONTROL 重複フィールド]**&#x200B;フィルターを探してキャンバスにドラッグします。

   ![](assets/three-4.png)

1. 次の 4 つのオプションの中から 1 つを選択します。

   * [!UICONTROL メールアドレス]
   * [!UICONTROL 姓名]
   * [!UICONTROL 名前（姓）]
   * [!UICONTROL 更新日時]

   >[!NOTE]
   >
   >「メールアドレス」を除くすべてのフィールドでは、大文字と小文字が区別されます。 したがって、「姓名」フィールドに「john doe」と入力すると、「John Doe」は結果に&#x200B;_返されません_。

   ![](assets/four-2.png)

   スマートリストを実行すると、あらかじめ選択したフィールドに同じ値を持つリードを検索できます。
