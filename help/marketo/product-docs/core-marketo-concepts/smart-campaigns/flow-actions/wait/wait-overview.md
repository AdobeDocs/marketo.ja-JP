---
unique-page-id: 1146950
description: 待機 — Marketto Docs — 製品ドキュメント
title: Wait
translation-type: tm+mt
source-git-commit: 29eb4c833c128c37849260f0c554144c237ab28e
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# 待機{#wait}

## 概要{#overview}

便利な&#x200B;**待機ステップ**&#x200B;を使用して、スマートキャンペーンフローで人を一時停止します。

![](assets/wait-overview.png)

「4時間」のような自然言語での入力方法に注目してください。 ただし、****&#x200B;を省略しないでください（4時間など）。 スマートキャンペーンは引き続き実行されますが、待機ステップは無視されます。

>[!CAUTION]
>
>待機ステップの期間を変更しても、既に入力されているユーザーには影響しません。 次に例を示します。5日間の待機ステップがある場合、ユーザーが入力した後、待機ステップを7日に変更します。そのユーザーは、元の5日間だけ待機してから次のフローステップに進みます。

>[!TIP]
>
>既に待機ステップに入っているユーザーが、待機期間が終了した後に進むことを望まない場合は、待機ステップの直後に[フローから削除](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md)を挿入します。 [選択肢](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-add-choice-in-a-flow-step.md)を追加オプションを使用して、削除するユーザーを指定します。

## 使用法{#usage}

待機フロー手順は、主に次の3つの方法で使用できます。

1. [待機フローステップでの期間の使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
1. [特定の日付を待機フロー・ステップで使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
1. [待機フロー手順での日付トークンの使用](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
