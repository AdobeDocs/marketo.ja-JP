---
unique-page-id: 2359449
description: セグメントルールの定義 — Marketto Docs — 製品ドキュメント
title: セグメントルールの定義
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---


# セグメントルールの定義{#define-segment-rules}

セグメントルールを定義すると、訪問者を様々な相互排他的なグループに分類できます。

>[!PREREQUISITES]
>
>[セグメントの作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. **データベースに移動します。**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. ツリーの&#x200B;**セグメント**&#x200B;をクリックし、特定の&#x200B;**セグメント**&#x200B;をクリックします。

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. **スマートリスト**&#x200B;をクリックし、フィルターを追加します。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >現在、セグメントでは、フィルターの&#x200B;_過去_&#x200B;および&#x200B;_時間枠_&#x200B;内演算子がサポートされていません。 これは、変更データ値がログに記録されるときにのみ、セグメント化で更新がチェックされるからです。 数式のフィールドや日付など、自動的に変更される値に対しては、__&#x200B;ログに記録されません。 また、相対的な日付範囲を持つ日付演算子は、データ値の変更アクティビティの時ではなく、セグメント化の承認時に計算されるので、サポートされません。

   >[!NOTE]
   >
   >「SFDC Type」と「Microsoft Type」のフィルターは、現在、セグメントスマートリストではサポートされていません。

1. フィルターに適切な値を入力します。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >スマートリストは素晴らしい。 [詳しくは、こちらを参照してください](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md)。

1. 「**人（ドラフト）**」タブをクリックして、このセグメントのメンバーになる資格を持つ人を表示します。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. **セグメント化アクション**&#x200B;に移動します。 「**承認**」をクリックします。

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >セグメントで作成できるセグメントの合計数は、使用するフィルターの数とタイプ、およびセグメントのロジックの複雑さによって異なります。 標準フィールドを使用して最大100個のセグメントを作成できますが、他のタイプのフィルターを使用すると複雑さが増し、セグメントを承認できない場合があります。 次に例を示します。カスタムフィールド、リストのメンバ、リード所有者フィールド、および売上高ステージ。
   >
   >承認中にエラーメッセージが表示され、セグメントの複雑さを軽減するために支援が必要な場合は、[マーケティング担当者](https://nation.marketo.com/t5/Support/ct-p/Support)にお問い合わせください。

1. 円グラフでセグメントの概要を簡単に確認するには、ダッシュボードと適用されるルールを確認します。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

お疲れさまでした！ これらのセグメントは、Marketoの多くの場所で役に立ちます。

>[!NOTE]
>
>1人の訪問者が異なるセグメントに属する可能性はありますが、最終的には、セグメント](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md)の[優先順位に依存するセグメントに属するだけです。

>[!NOTE]
>
>人（ドラフト）画面には、会員資格を持つすべての人が表示され、必ずしも人の最終リストとは限りません。 セグメントを承認して、最終リストを確認します。

>[!MORELIKETHIS]
>
>[セグメントの承認](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
