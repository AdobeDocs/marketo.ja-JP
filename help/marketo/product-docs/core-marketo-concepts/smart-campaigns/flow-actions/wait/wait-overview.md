---
unique-page-id: 1146950
description: 待機 - Marketo ドキュメント - 製品ドキュメント
title: 待機
exl-id: 58f43c4b-6f20-4740-9a25-e09c7ea31dcf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 100%

---

# 待機 {#wait}

## 概要 {#overview}

便利な&#x200B;**待機ステップ**&#x200B;を使用して、スマートキャンペーンのフロー内にいるリードの進行を停止できます。

![](assets/wait-overview.png)

「4 hours」のように、自然な言葉で入力できることに注目してください。ただし、省略形は&#x200B;**使用しない**&#x200B;でください（例：4 hrs）。スマートキャンペーンは引き続き実行されますが、待機ステップは無視されます。

>[!CAUTION]
>
>待機ステップの期間を変更しても、既に待機中のリードには影響しません。例：5 日間の待機ステップにリードが進行した後で、待機期間が 7 日間に変更された場合、リードは次のフローステップに進むまで、もともと指定されていた 5 日間にわたり待機します。

>[!TIP]
>
>既に待機ステップにいるリードが、待機期間が終了したときに進行しないようにする場合は、待機ステップの直後に「[フローから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)」を挿入します。「[選択肢を追加](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md)」オプションを使用して、削除するリードを指定します。

## 使用方法 {#usage}

待機フローステップには、次の 3 つの用途があります。

1. [待機フローステップで停止期間を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [待機フローステップで特定の日付を使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [待機フローステップで日付トークンを使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
