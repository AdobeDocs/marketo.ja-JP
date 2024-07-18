---
unique-page-id: 557316
description: スマートリストフィルターの定義 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストフィルターの定義
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 36%

---

# スマートリストフィルターの定義 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [フィルターを検索してスマートリストに追加する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

[ スマートリストを作成 ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} して [ フィルターを追加 ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} したので、フィルターを定義します。 手順は以下のとおりです。

この例では、次のフィルターを定義して、カリフォルニア州在住で、スコアが 50 を超える人をすべて検索します。

1. 「**[!UICONTROL マーケティングアクティビティ]**」に移動します。

   ![](assets/define-smart-list-filters-1.png)

1. 目的のスマート・リストを選択し、「**[!UICONTROL スマート・リスト]**」タブをクリックします。

   ![](assets/define-smart-list-filters-2.png)

1. 「状態 ]**フィルターの「CA**[!UICONTROL  を検索して選択します。

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >「California」と「CA」の両方を保存している可能性があります。 両方の値をフィルタし、カリフォルニア州の _すべて_ の人を含めるには、[ スマート・リスト・フィルタに複数の値を追加する ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"} 方法を説明します。

1. **[!UICONTROL 次より大きい]** 演算子を選択して、「50」と入力します。

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>データベースに不完全なメールアドレスを含むレコード（例：単に「@adobe.com」）があると思われる場合、「contains」演算子を使用する際には、2 つのメールアドレスフィルターを使用します。 1 つは「@adobe.com」を含むフィルターで、もう 1 つは「adobe.com」（@記号は除く）を含むフィルターです。

これで、スマートリストを作成してフィルターを追加または定義する方法がわかりました。
