---
unique-page-id: 1146901
description: 高度なスマートリストルールロジック — Marketto Docs — 製品ドキュメントの使用
title: 高度なスマートリスト・ルール・ロジックの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# 高度なスマートリスト・ルール・ロジックの使用 {#using-advanced-smart-list-rule-logic}

スマートリスト内の複数のフィルターにスマートリストルールロジックを適用すると、必要な人物を正確に検索できます。 これが方法です。

>[!PREREQUISITES]
>
>* [スマート・リストの検索と追加フィルター](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [スマートリストフィルターの定義](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>



>[!NOTE]
>
>アドバンスフィルターロジックは、スマートリストに3つ以上のフィルターがある場合にのみ使用できます。

## スマートリスト追加へのロジック {#add-logic-to-a-smart-list}

デフォルトでは、スマートリストは **ALL** フィルター(フィルター1 *と* 2 *と* 3)に一致する人を検索します。 ルールロジックを変更して、定義済みのフィルター **(フィルター1または** 2 *、3)の* ANYに一致する訪問者を検索したり、高度なフィルター(フィルター1 **** および2または*3)を使用したりできます。

この例では、カリフォルニア州で、50ポイント以上 *のスコアを持つ*** 、または「Sales Qualified」のステータスを持つ人を探すとします。

1. ドロップダウンから **「** アドバンス **フィルターを使用****** 」を選択します。

   ![](assets/one.png)

   >[!NOTE]
   >
   >アド **バンス** ・フィルターを使用すると、スマート・リストのメンバー・フィルタを使用してスマート・リストを作成する必要が少なくなります。 これにより、パフォーマンスを最適化できます。

1. 「 **詳細****フィルター** 」テキストボックスに、すべてのフィルター間のデフォルト値として「and」が表示されます。

   ![](assets/two-2.png)

1. 「2と3」を括弧で囲んで入力します。

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >ルールロジックを入力する際は、「or」の前に「and」を使用する必要があります。

1. 「and」を「2」から「3」に変更して、「or」にします。

   ![](assets/four-1.png)

## 「And」と「Or」を混在させる場合は丸括弧を使用 {#use-parentheses-when-mixing-and-and-or}

「and」と「or」のロジックを混在させる場合、意図を明確にするには括弧が必要です。

![](assets/advancedfilters-parent.png)

## 必要に応じて4つ以上のフィルターに入れ子の丸括弧を使用 {#use-nested-parentheses-for-four-or-more-filters-if-needed}

意図に応じて、4つ以上のフィルターを使用する場合は、入れ子の丸括弧の追加が必要になる場合があります。

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>無効なルールを入力すると、そのルールの下に赤い線が表示されます。 テキストをスクロールすると、関連するエラーメッセージが表示されます。

