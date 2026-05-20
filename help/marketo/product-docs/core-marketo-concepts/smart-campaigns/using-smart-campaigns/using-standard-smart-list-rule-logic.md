---
unique-page-id: 1147001
description: スマートキャンペーンで標準のスマートリストルールロジックを使用する方法を説明します。 フィルターをAND ロジックと組み合わせて選定します。
title: 標準スマートリストルールロジックの使用
exl-id: 9befaa81-e50c-47d3-9edf-220cfadd00f6
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/hRPdzjEUOeC2PZK2YlO1IPZOPoPOfo7CHJu2yUtU0qc
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 60%

---

# 標準スマートリストルールロジックの使用 {#using-standard-smart-list-rule-logic}

キャンペーンのスマートリストを作成する際に、「フィルターを使用」オプションに気づいたかもしれません。 この設定を使用すると、フィルターを AND または OR 演算子で評価する必要があるかどうかを決定できます。

![](assets/using-standard-smart-list-rule-logic-1.png)

>[!NOTE]
>
>スマートリストルールロジックの変更は、フィルターのみに適用され、トリガーには&#x200B;_適用されません_。

上記の設定がALLに設定されている場合でも、トリガーは常にORとして評価されます。 例：

![](assets/using-standard-smart-list-rule-logic-2.png)

上記のスマートリストを単語で表します。

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
