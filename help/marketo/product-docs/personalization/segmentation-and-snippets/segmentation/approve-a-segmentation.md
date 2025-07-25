---
unique-page-id: 2359457
description: セグメント化の承認 - Marketo ドキュメント - 製品ドキュメント
title: セグメント化の承認
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '232'
ht-degree: 89%

---

# セグメント化の承認 {#approve-a-segmentation}

セグメントを使用するには、セグメント化の承認が必要です。

>[!PREREQUISITES]
>
>* [セグメント化の作成](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md)
>* [セグメントルールの定義](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)

>[!NOTE]
>
>一度に承認できるセグメント化は最大 20 個です。

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/image2017-3-28-14-3a25-3a49.png)

1. セグメント化で、**[!UICONTROL セグメント化アクション]**／**[!UICONTROL 承認]**&#x200B;をクリックします。

   ![](assets/image2017-3-28-14-3a46-3a22.png)

   >[!NOTE]
   >
   >承認の処理中、ステータスが [!UICONTROL &#x200B; 承認中 &#x200B;] に変わり、回転輪（![](assets/image2014-9-15-15-3a31-3a43.png)）が表示されます。

   >[!CAUTION]
   >
   >データベースのサイズによっては、承認が完了するまでに数分かかり、1 日以上かかる場合があります。

   承認が完了すると、[!UICONTROL &#x200B; ステータス &#x200B;] が [!UICONTROL &#x200B; 承認中 &#x200B;] から [!UICONTROL &#x200B; 承認済み &#x200B;] に変わります。
   ![](assets/image2017-3-28-14-3a46-3a44.png)

   >[!TIP]
   >
   >各セグメントのユーザー数は、括弧で囲まれてセグメント名の横に表示されます。

1. **[!UICONTROL セグメント]**&#x200B;の「**[!UICONTROL リード]**」タブで、セグメントの最終的なリードリストが表示されます。

   ![](assets/image2017-3-28-14-3a47-3a10.png)

>[!CAUTION]
>
>セグメント化で作成できるセグメントの合計数は、使用するフィルターの数と種類と、セグメントのロジックの複雑さによって異なります。標準フィールドを使用して最大 100 個のセグメントを作成できますが、他のタイプのフィルターを使用すると複雑さが増し、セグメント化を承認できない場合があります。例は、カスタムフィールド、リストのメンバー、リード所有者フィールド、収益ステージです。
>
>承認中にエラーメッセージが表示され、セグメント化の複雑さを軽減するためにサポートが必要な場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に問い合わせてください。

>[!MORELIKETHIS]
>
>[スマートリストでのセグメントフィルターの使用](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
