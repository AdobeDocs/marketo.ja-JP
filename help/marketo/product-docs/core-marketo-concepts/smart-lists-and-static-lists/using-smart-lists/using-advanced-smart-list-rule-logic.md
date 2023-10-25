---
unique-page-id: 1146901
description: 高度なスマートリストルールロジックの使用 - Marketo ドキュメント - 製品ドキュメント
title: 高度なスマートリストルールロジックの使用
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 75%

---

# 高度なスマートリストルールロジックの使用 {#using-advanced-smart-list-rule-logic}

スマートリスト内の複数のフィルターにスマートリストルールロジックを適用すると、必要な人物を見つけることができます。 手順は以下のとおりです。

>[!PREREQUISITES]
>
>* [フィルターを検索してスマートリストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}
>* [スマートリストフィルターの定義](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md){target="_blank"}

>[!NOTE]
>
>詳細フィルターロジックは、スマートリストに 3 つ以上のフィルターがある場合にのみ使用できます。

## スマートリストへのロジックの追加 {#add-logic-to-a-smart-list}

デフォルトでは、スマートリストは一致する人を検索します **[!UICONTROL すべて]** フィルタ（フィルタ 1） _および_ 2 _および_ 3)。 ルールロジックを変更して、定義済みフィルターの&#x200B;**[!UICONTROL いずれか]**（フィルター 1 _または_ 2 _または_ 3）に一致するユーザーを検索する、または詳細フィルター（フィルター 1 _および_ 2 _または_ 3）を使用することができます。

この例では、カリフォルニア州にいる&#x200B;_および_、スコアが 50 ポイント&#x200B;_または_&#x200B;ステータスが「Sales Qualified」であるリードを検索するとします。

1. ドロップダウンから「**[!UICONTROL 詳細フィルター]**&#x200B;を使用」を選択します。

   ![](assets/one.png)

   >[!NOTE]
   >
   >使用 **[!UICONTROL 詳細]** フィルタは、スマートリストのメンバーフィルタを使用してスマートリストを作成する必要を減らします。 これは、パフォーマンスの最適化に役立ちます。

1. 「**[!UICONTROL 詳細フィルター]**」テキストボックスには、すべてのフィルターのデフォルト値として「and」が表示されます。

   ![](assets/two-2.png)

1. 「2 and 3」を囲むように丸括弧を入力します。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >ルールロジックを入力する際は、「or」の前に「and」を使用する必要があります。

1. 「2 and 3」の「and」を「or」に変更します。

   ![](assets/four-1.png)

## 「and」と「or」を混在させる場合は括弧を使用する {#use-parentheses-when-mixing-and-and-or}

「and」と「or」のロジックを組み合わせるには、意図を明確にするための括弧が必要です。

![](assets/advancedfilters-parent.png)

## 必要に応じて、4 つ以上のフィルターにネストされた括弧を使用する {#use-nested-parentheses-for-four-or-more-filters-if-needed}

目的に応じて、4 つ以上のフィルターを使用する場合は、ネストされた括弧を追加する必要が生じる場合があります。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>無効なルールを入力すると、そのルールの下に赤い線が表示されます。テキストの上にスクロールすると、関連するエラーメッセージが表示されます。
