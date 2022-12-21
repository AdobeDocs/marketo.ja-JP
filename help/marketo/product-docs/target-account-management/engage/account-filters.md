---
unique-page-id: 11380732
description: 顧客フィルター - Marketo ドキュメント - 製品ドキュメント
title: 顧客フィルター
exl-id: a359f53b-c0a0-4b46-bad0-2840ba668892
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 100%

---

# 顧客フィルター {#account-filters}

新しい顧客中心型フィルターを使用して、重点顧客とその中の人物を特定し、惹きつけます。

## TAM フィルター {#tam-filters}

1. 目的のスマートキャンペーンに移動して「**スマートリスト**」をクリックします。

   ![](assets/one.png)

1. 「**+**」をクリックして、**顧客フィルター**&#x200B;フォルダーを展開します。

   ![](assets/two.png)

1. 使用するフィルターをキャンバスにドラッグします。

   ![](assets/three.png)

## 顧客リストのメンバー {#member-of-account-list}

このフィルターを使用するには、顧客リストドロップダウンをクリックして、

![](assets/four.png)

目的の顧客リストを選択します。

![](assets/five.png)

>[!NOTE]
>
>「顧客リストのメンバー」フィルターにある修飾子は「is」 1 つだけです。追加の修飾子（「is not」や「is any」など）は使用できません。

## 重点顧客のメンバー {#member-of-named-account}

まず、修飾子を選択します。特定の重点顧客の場合は **Is**、任意の重点顧客の場合は **is any** です。

![](assets/six.png)

重点顧客ドロップダウンをクリックして、

![](assets/seven.png)

目的の重点顧客を選択します。

![](assets/eight.png)

「is any」修飾子を使用する場合、[制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)を使用して検索結果を絞り込むことをおすすめします。必要な数だけ追加してください。

![](assets/nine.png)

単一の最上位顧客からのみメンバーを取得する場合は、「子を含める」を false に設定します。すべての子顧客からメンバーを取得する場合は、true を選択します。

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[顧客トリガー](/help/marketo/product-docs/target-account-management/engage/account-triggers.md)
