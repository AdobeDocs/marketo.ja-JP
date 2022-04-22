---
unique-page-id: 2359449
description: セグメントルールの定義 - Marketo ドキュメント - 製品ドキュメント
title: セグメントルールの定義
exl-id: e6631848-aa8c-4709-b182-4c88abbd365b
source-git-commit: 55afdc537d0a5d0b6114f478c4dd2ded09c84e34
workflow-type: ht
source-wordcount: '382'
ht-degree: 100%

---

# セグメントルールの定義 {#define-segment-rules}

セグメントルールを定義すると、顧客を異なる相互に排他的なグループに分類できます。

>[!PREREQUISITES]
>
>[セグメント化の作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)

1. **データベース**&#x200B;に移動します。

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. ツリーから「**セグメント化**」を選択し、特定の&#x200B;**セグメント**&#x200B;をクリックします。

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. 「**スマートリスト**」をクリックして、フィルターを追加します。

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >セグメントは現在、フィルターの _In Past_ および _In Timeframe_ 演算子をサポートしていません。これは、セグメント化では、変更データ値がログに記録されたときにのみ更新を確認するためです。これらの値は、数式フィールドや日付など、自動的に変更される項目に対してログに記録され&#x200B;_ません_。また、相対的な日付範囲を持つ日付演算子は、データ値の変更アクティビティの時点ではなく、セグメント化の承認時に計算されるので、サポートされません。

   >[!NOTE]
   >
   >「SFDC タイプ」および「Microsoft タイプ」フィルターは、現在、スマートリストのセグメント化ではサポートされていません。

1. フィルターに適切な値を入力します。

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!CAUTION]
   >
   >アカウントフィールドのアクティビティログの動作は、認定に影響を与える可能性があります。したがって、セグメントルールを定義する際には、アカウントフィールドを使用しないことをお勧めします。

1. 「**リード（ドラフト）**」タブをクリックすると、このセグメントのメンバーになる資格のあるリードが表示されます。

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. **セグメント化アクション**&#x200B;に移動します。「**承認**」をクリックします。

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >セグメントで作成できるセグメントの合計数は、使用するフィルターの数と種類と、セグメントのロジックの複雑さによって異なります。標準フィールドを使用して最大 100 個のセグメントを作成できますが、他のタイプのフィルターを使用すると複雑さが増し、セグメント化を承認できない場合があります。例は、カスタムフィールド、リストのメンバー、リード所有者フィールド、収益ステージです。
   >
   >承認中にエラーメッセージが表示され、セグメント化の複雑さを軽減するためにサポートが必要な場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に問い合わせてください。

1. ダッシュボードでは、円グラフでのセグメントおよび適用されたルールの概要をすばやく確認できます。

   ![](assets/image2014-9-15-11-3a36-3a19.png)

お疲れさまでした。これらのセグメントは Marketo の多くの場所で役に立つでしょう。

>[!NOTE]
>
>ユーザーは様々なセグメントに適合する場合がありますが、最終的には、[セグメントの優先順位](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md)に従って 1 つのみに属するようになります。

>[!NOTE]
>
>リード（ドラフト）画面には、メンバーとして認定されるすべてのユーザーが表示され、必ずしもユーザーの最終リストとは限りません。セグメントを承認すると、最終リストを確認できます。

>[!MORELIKETHIS]
>
>[セグメント化の承認](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md)
