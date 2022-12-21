---
unique-page-id: 557316
description: スマートリストフィルターの定義 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストフィルターの定義
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 100%

---

# スマートリストフィルターの定義 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [スマートリストの作成](create-a-smart-list.md)
>* [フィルターを検索してスマートリストに追加する](find-and-add-filters-to-a-smart-list.md)


[スマートリストを作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)し、[フィルターを追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)できたので、フィルターを定義しましょう。手順は以下のとおりです。

この例では、次のフィルターを定義して、カリフォルニア州在住で、スコアが 50 を超える人をすべて検索します。

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. スマートリストを選択し、「**スマートリスト**」タブをクリックします。

   ![](assets/smarlist-choosefilters.png)

1. 「**州**」フィルターから「**CA**」を検索して選択します。

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >**カリフォルニア**&#x200B;および **CA**.の両方が保存されている可能性があります。両方の値に対してフィルターを適用して、カリフォルニア州在住の人を&#x200B;_すべて_&#x200B;含めるには、[スマートリストフィルターへの複数値の追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md)を参照してください。

1. **指定の値より大きい**&#x200B;演算子を選び、**50** と入力します。

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>不完全なメールアドレス（例：「@adobe.com」のみ）を含むレコードがデータベースに存在する可能性がある場合は、「次を含む」演算子を使用する際に、**2** つのメールアドレスフィルターを使用します。1 つは「@adobe.com」を含むフィルターで、もう 1 つは「adobe.com」（@記号は除く）を含むフィルターです。

スマートリストを作成し、フィルターを追加／定義する方法がわかりました。
