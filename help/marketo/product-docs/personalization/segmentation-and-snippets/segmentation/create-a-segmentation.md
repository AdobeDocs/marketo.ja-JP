---
unique-page-id: 2359447
description: レポートと動的コンテンツ用にユーザーをグループ化するセグメンテーションを作成する方法について説明します。 データベースでセグメントを追加し、順序を設定してから、セグメントルールを定義します。
title: セグメント化の作成
exl-id: a7907f1d-bc78-4b63-9875-044e96609755
feature: Segmentation
TQID: https://experienceleague.adobe.com/Xp4uo4aDMkK9Di3Dp0ufHnxgg8ci7YDD2qOO6rZwI7M
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2:
  - id: a1d50dda-6d94-4e16-8c30-5eb7181c4650
  - id: cdd4e0f6-e87e-453f-88ee-2ee54a7de272
  - id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 246
ht-degree: 90%

---

# セグメント化の作成 {#create-a-segmentation}

セグメント化を使用すると、レポートや動的コンテンツ用に、個々のユーザーを別々のプロファイルにグループ化できます。 作成する方法は、以下のとおりです。

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/create-a-segmentation-1.png)

1. 「**[!UICONTROL 新規]**」をクリックし、次に「**[!UICONTROL 新規セグメント化]**」をクリックします。

   ![](assets/create-a-segmentation-2.png)

   >[!TIP]
   >
   >最大 20 個のセグメント化を作成できます。

1. **[!UICONTROL 名前]**&#x200B;を入力し、「**[!UICONTROL セグメントを追加]**」をクリックして名前を付けます。

   ![](assets/create-a-segmentation-3.png)

   >[!NOTE]
   >
   >デフォルトは移動、編集、削除できません。

1. 必要な数のセグメントを追加します（最大 100 個）。

   ![](assets/create-a-segmentation-4.png)

   >[!CAUTION]
   >
   >セグメント化で作成できるセグメントの合計数は、使用するフィルターの数と種類と、セグメントのロジックの複雑さによって異なります。 標準フィールドを使用して最大 100 個のセグメントを作成できますが、他のタイプのフィルターを使用すると複雑さが増し、セグメント化を承認できない場合があります。 例は、カスタムフィールド、リストのメンバー、リード所有者フィールド、収益ステージです。
   >
   >承認中にエラーメッセージが表示され、セグメント化の複雑さを軽減するためにサポートが必要な場合は、[Marketo サポート](https://nation.marketo.com/t5/Support/ct-p/Support)に問い合わせてください。

1. セグメントをドラッグ＆ドロップして順序を変更します。 完了したら、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/create-a-segmentation-5.png)

   >[!NOTE]
   >
   >リードは、定義された[順序](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md)で最初に一致するセグメントの資格を得ることになります。

   >[!NOTE]
   >
   >セグメント化を使用する前に、セグメントルールを定義する必要があります。

   これで完了です。 動的コンテンツの使用に一歩近づきました。

   >[!MORELIKETHIS]
   >
   >[セグメントルールの定義](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
