---
unique-page-id: 1147001
description: 標準スマートリストルールロジックの使用 - Marketo ドキュメント - 製品ドキュメント
title: 標準スマートリストルールロジックの使用
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 73%

---

# 標準スマートリストルールロジックの使用 {#using-standard-smart-list-rule-logic}

Campaign スマートリストを作成する際に、「フィルターを使用」オプションに気付いた可能性があります。 この設定を使用すると、フィルターを AND または OR 演算子で評価する必要があるかどうかを決定できます。

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>スマートリストルールロジックの変更は、フィルターのみに適用され、トリガーには&#x200B;_適用されません_。

上記の設定が ALL に設定されている場合でも、トリガーは常にまたはと評価されます。 次に例を示します。

![](assets/using-standard-smart-list-rule-logic-2.png)

上記のスマートリストは次の語句で表されます。

```box
IF person fills out Great Form
OR
IF person visits Keith's Landing Page
AND
Industry is Energy
AND
Country is US
THEN follow the campaign's flow step(s)
```

したがって、人物がフォームに入力する&#x200B;_または_&#x200B;ページを訪問すると、キャンペーンは、後続のフィルターの&#x200B;_すべて_&#x200B;または&#x200B;_いずれか_&#x200B;を基に人物を評価します（使用する設定に応じます）。

>[!MORELIKETHIS]
>
>[高度なスマートリストルールロジックの使用](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md){target="_blank"}
