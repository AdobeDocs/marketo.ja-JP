---
unique-page-id: 1146980
description: フロー手順追加での選択肢の使用 — Marketto Docs — 製品ドキュメント
title: フローステップでの追加選択の使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# フローステップでの追加選択の使用 {#use-add-choice-in-a-flow-step}

>[!PREREQUISITES]
>
>* [スマ追加ートキャンペーンへのフローステップ](add-a-flow-step-to-a-smart-campaign.md)

>



**追加選択すると** 、フローステップを使用して、詳細を選択する際に「次に依存する」と答えることができます。

1. スマートキャンペーンの「 **フロー** 」タブで、フローステップを追加し、「 **追加選択**」をクリックします。

   ![](assets/image2014-9-22-11-3a58-3a20.png)

1. 選択条件を選択します。

   ![](assets/image2014-9-22-11-3a58-3a50.png)

1. 選択演算子を選択し、選択値を入力します。 条件または選択肢が設定されます。

   ![](assets/image2014-9-22-11-3a58-3a54.png)

1. 選択肢のフローステップの値を入力します。

   ![](assets/image2014-9-22-11-3a58-3a57.png)

   >[!CAUTION]
   >
   >トークンは、選択フロー手順の条件部分では **機能しません** 。

1. 上記の手順を繰り返して複数の選択肢を追加し、デフォルト値を追加/調整します。

   ![](assets/image2014-9-22-11-3a58-3a59.png)

   >[!TIP]
   >
   >フローステップを —Do Nothing — に設定すると、その選択に対して何も実行されません。

   >[!CAUTION]
   >
   >最初に一致した選択肢のみがフローステップに適用されます。 フローアクションの「追加選択」の [順序を変更する方法を説明します](reorder-add-choice-in-a-flow-step.md)。

   >[!NOTE]
   >
   >**関連記事**
   >
   >    
   >    
   >    * [フローステップの「追加選択」の並べ替え](reorder-add-choice-in-a-flow-step.md)


素晴らしい！ 各選択肢に対して複数のスマートキャンペーンを作成する代わりに、フローステップの選択肢を持つ1つのスマートキャンペーンを作成できるようになりました。