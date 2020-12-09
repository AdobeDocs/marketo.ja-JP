---
unique-page-id: 1147001
description: 標準的なスマートリストルールロジックの使用 — Marketto Docs — 製品ドキュメント
title: 標準スマート・リスト・ルール・ロジックの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# 標準スマート・リスト・ルール・ロジックの使用 {#using-standard-smart-list-rule-logic}

キャンペーンのスマートリストを構築する際に、「フィルターを使用」オプションが表示されている可能性があります。 この設定を使用すると、フィルターをANDまたはOR演算子で評価する必要があるかどうかを判断できます。

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

![](assets/image2014-9-22-14-3a12-3a42.png)

>[!NOTE]
>
>スマートリストルールロジックの変更は、フィルターにのみ適用され、トリガー **には適用されません** 。

上記の設定がALLに設定されている場合でも、トリガーは常にORとして評価されます。  次に例を示します。

![](assets/image2014-9-22-14-3a12-3a57.png)

上記のスマートリスト（単語）:`<pre data-theme="Confluence">IF person fills out My Form OR IF person visits My Page AND Industry is Marketing AND Country is USA THEN follow the campaign's flow step(s)</pre>` したがって、ユーザーがフォームに入力した **** かページを訪問した場合、キャンペーンは、使用した設定に応じて、後続のフィルターの**all **or **any **に基づいてそのユーザーを評価します。

>[!MORELIKETHIS]
>
>* [高度なスマートリスト・ルール・ロジックの使用](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/using-advanced-smart-list-rule-logic.md)

>



