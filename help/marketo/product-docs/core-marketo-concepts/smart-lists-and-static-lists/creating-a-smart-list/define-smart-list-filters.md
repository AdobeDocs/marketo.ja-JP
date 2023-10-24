---
unique-page-id: 557316
description: スマートリストフィルターの定義 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストフィルターの定義
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 53%

---

# スマートリストフィルターの定義 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [フィルターを検索してスマートリストに追加する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

これで、 [スマートリストを作成しました](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} and [added filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} それに対して、フィルターを定義します。 手順は以下のとおりです。

この例では、次のフィルターを定義して、カリフォルニア州在住で、スコアが 50 を超える人をすべて検索します。

1. 「**[!UICONTROL マーケティングアクティビティ]**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. スマートリストを選択し、 **[!UICONTROL スマートリスト]** タブをクリックします。

   ![](assets/smarlist-choosefilters.png)

1. を検索し、「CA」を選択します。 **[!UICONTROL 都道府県]** フィルター。

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >「カリフォルニア」と「CA」の両方を保存している可能性があります。 両方の値に対してフィルターを適用し、次の値を含めます。 _すべて_ カリフォルニア出身の人々は、次の方法を学びます。  [スマートリストフィルタに複数の値を追加する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. 次を選択： **[!UICONTROL 次よりも大きい]** 演算子を使用して「50」と入力します。

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>不完全なメールアドレス（例：「@adobe.com」のみ）を含むレコードがデータベースに存在する可能性がある場合は、「次を含む」演算子を使用する際に、2 つのメールアドレスフィルターを使用します。1 つは「@adobe.com」を含むフィルターで、もう 1 つは「adobe.com」（@記号は除く）を含むフィルターです。

これで、スマートリストを作成し、フィルターを追加/定義する方法がわかりました。
