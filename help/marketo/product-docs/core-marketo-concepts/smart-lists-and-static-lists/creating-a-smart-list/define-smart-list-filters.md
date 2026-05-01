---
unique-page-id: 557316
description: スマートリストフィルターの定義方法を説明します。 フィルターの制約と値を設定して、リストに表示されるユーザーを決定します。
title: スマートリストフィルターの定義
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 56%

---

# スマートリストフィルターの定義 {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [スマートリストの作成](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [フィルターを検索してスマートリストに追加する](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

これで、[ スマートリストを作成し](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} フィルターを[追加しました](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}。次のようにフィルターを定義します。

この例を続けて、これらのフィルターを定義して、スコアが50を超えるカリフォルニアのすべてのユーザーを検索します。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/define-smart-list-filters-1.png)

1. 目的のスマートリストを選択し、「**[!UICONTROL スマートリスト]**」タブをクリックします。

   ![](assets/define-smart-list-filters-2.png)

1. 「**[!UICONTROL 州]**」フィルターから「CA」を検索して選択します。

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >「カリフォルニア」および「CA」の両方が保存されている可能性があります。 両方の値に対してフィルターを適用して、カリフォルニア州在住の人を&#x200B;_すべて_&#x200B;含めるには、[スマートリストフィルターへの複数値の追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}を参照してください。

1. **[!UICONTROL 指定の値より大きい]**&#x200B;演算子を選び、「50」と入力します。

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>不完全な電子メールアドレスを含むレコードがデータベースに存在する可能性があると思われる場合（例：「@adobe.com」）、「contains」演算子を使用する場合は、2つの電子メールアドレスフィルターを使用します。 1 つは「@adobe.com」を含むフィルターで、もう 1 つは「adobe.com」（@ 記号は除く）を含むフィルターです。

これで、スマートリストを作成し、フィルターを追加／定義する方法がわかりました。
