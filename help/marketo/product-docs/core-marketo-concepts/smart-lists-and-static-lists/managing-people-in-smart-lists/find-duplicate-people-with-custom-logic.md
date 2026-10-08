---
unique-page-id: 2952636
description: カスタムロジックを使用して重複するユーザーを見つける方法を説明します。 スマートリストを作成し、基準ごとに重複を識別できます。
title: カスタムロジックを使用した重複人物の検索
exl-id: e268ca34-03a3-403a-8869-4e2b60bba05c
feature: Smart Lists
TQID: 'https://experienceleague.adobe.com/-NvWt-eEzngL0QY7Kyl6lfjd75WcoQmcq3IiN7Uc6-w'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 77%
---
# カスタムロジックを使用した重複人物の検索 {#find-duplicate-people-with-custom-logic}

Adobe Marketo Engage には、メールアドレスを照合して重複する人物を見つけるシステムスマートリストがあります。 別のフィールドを使用して、との重複を見つける場合は、次の手順に従います。

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

   スマートリストを実行すると、あらかじめ選択したフィールドに同じ値を持つ人物を検索できます。
