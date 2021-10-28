---
unique-page-id: 2359457
description: セグメント化の承認 — Marketoドキュメント — 製品ドキュメント
title: セグメント化の承認
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
source-git-commit: 0a1e913fd03415d3668c8a9d2200e2211bad5980
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 12%

---

# セグメント化の承認 {#approve-a-segmentation}

セグメントを使用するには、セグメント化の承認が必要です。

>[!PREREQUISITES]
>
>* [セグメント化の作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [セグメントルールの定義](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)


>[!NOTE]
>
>一度に承認できるセグメントは最大 20 個です。

1. **データベース**&#x200B;に移動します。

   ![](assets/image2017-3-28-14-3a25-3a49.png)

1. セグメントで、 **セグメント化アクション**、 **承認**.

   ![](assets/image2017-3-28-14-3a46-3a22.png)

   >[!NOTE]
   >
   >「ステータス」が「スピンホイールを使用した承認」( ![](assets/image2014-9-15-15-3a31-3a43.png)) をクリックします。

   >[!CAUTION]
   >
   >データベースのサイズによっては、承認が完了するまでに数分かかり、1 日以上かかる場合があります。

   承認が完了すると、「ステータス」は「承認中」から「承認済み」に変わります。
   ![](assets/image2017-3-28-14-3a46-3a44.png)

   >[!TIP]
   >
   >各セグメントのユーザー数は、括弧で囲まれてセグメント名の横に表示されます。

1. この **人** 」タブをクリックします。 **セグメント** では、セグメントの最終的なリストが表示されます。

   ![](assets/image2017-3-28-14-3a47-3a10.png)

>[!CAUTION]
>
>セグメントで作成できるセグメントの合計数は、使用するフィルターの数と種類と、セグメントのロジックの複雑さによって異なります。 標準フィールドを使用して最大 100 個のセグメントを作成できますが、他のタイプのフィルターを使用すると複雑さが増し、セグメントを承認できない場合があります。 次に例を示します。カスタムフィールド、リストのメンバー、リード所有者フィールド、収益ステージ。
>
>承認中にエラーメッセージが表示され、セグメント化の複雑さを軽減するためにサポートが必要な場合は、 [Marketoサポート](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!MORELIKETHIS]
>
>[スマートリストでのセグメントフィルターの使用](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
