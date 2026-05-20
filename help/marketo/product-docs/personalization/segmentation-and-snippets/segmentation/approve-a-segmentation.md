---
unique-page-id: 2359457
description: 動的なコンテンツとレポートに使用できるように、セグメンテーションを承認する方法を説明します。 セグメントルールを定義した後で、データベースとセグメント化アクションを使用して承認します。
title: セグメント化の承認
exl-id: c8b0fbe9-012c-47bf-8769-0167156b43d3
feature: Segmentation
TQID: https://experienceleague.adobe.com/hvFKybwLh1INYx2YWtOmdebJVYXOzhNMMncqeOoV8EU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 76%

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

   ![](assets/approve-a-segmentation-1.png)

1. セグメント化で、**[!UICONTROL セグメント化アクション]**／**[!UICONTROL 承認]**&#x200B;をクリックします。

   ![](assets/approve-a-segmentation-2.png)

   >[!NOTE]
   >
   >承認の処理中にステータスが&#x200B;_承認中_&#x200B;に変更されます。

   >[!CAUTION]
   >
   >承認は、データベースのサイズに応じて、数分から1日または2日かかることがあります。

1. 承認が完了すると、[!UICONTROL ステータス]は「[!UICONTROL 承認中]」から「[!UICONTROL 承認済み]」に変わります。

   ![](assets/approve-a-segmentation-3.png)

   >[!TIP]
   >
   >各セグメントのユーザー数は、括弧で囲まれてセグメント名の横に表示されます。

1. **[!UICONTROL セグメント]**&#x200B;の「**[!UICONTROL リード]**」タブで、セグメントの最終的なリードリストが表示されます。

   ![](assets/approve-a-segmentation-4.png)

>[!CAUTION]
>
>セグメント化で作成できるセグメントの合計数は、使用するフィルターの数と種類と、セグメントのロジックの複雑さによって異なります。 標準フィールドを使用して最大 100 個のセグメントを作成できますが、他のタイプのフィルターを使用すると複雑さが増し、セグメント化を承認できない場合があります。 例は、カスタムフィールド、リストのメンバー、リード所有者フィールド、収益ステージです。
>
>承認中にエラーメッセージが表示され、セグメント化の複雑さを軽減するためにサポートが必要な場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に問い合わせてください。

>[!MORELIKETHIS]
>
>[スマートリストでのセグメントフィルターの使用](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/use-segment-filters-in-a-smart-list.md)
