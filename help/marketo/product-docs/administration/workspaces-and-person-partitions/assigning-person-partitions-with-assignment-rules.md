---
unique-page-id: 2360327
description: 割り当てルールを使用した個人パーティションの割り当て — Marketto Docs — 製品ドキュメント
title: 割当ルールを使用した個人パーティションの割当
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# 割当ルールを使用した個人パーティションの割当 {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**FYI**
>
>Marketoは現在、すべての購読で言語を標準化しているので、購読およびdocs.marketo.comの人物/人物にリード/リードを表示できます。 これらの用語は同じことを意味し、記事の説明には影響しません。 他にも変化がある。 [詳細情報](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**必要な管理者権限**

>[!NOTE]
>
>**前提条件**
>
>* [個人パーティションの作成](create-a-person-partition.md)

>



個人パーティションを使用する場合、CRMから作成された個人をそれぞれのパーティションにルーティングする割り当てルールを設定します。

>[!NOTE]
>
>CRMから、およびSOAP APIを介してMarketorで作成された人のみに、割り当てルールが適用されます。

1. 「管理者」で、「ワークスペースとパーティション」をクリックします。

![](assets/image2014-9-17-10-3a32-3a55.png)

1. 「**ユーザー・パーティション**」タブで、「 **割当ルール**」をクリックします。

   ![](assets/two-6.png)

1. 「**追加選択**」をクリックして、個人パーティションにルーティングユーザーの条件を追加します。

   ![](assets/three-6.png)

1. 条件を作成するフィールドを選択します。

   ![](assets/four-5.png)

1. 選択演算子を選択し、値を入力します。
1. ![](assets/five-1.png)

1. 条件を満たすユーザーを分類するユーザーパーティションを選択します。

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >
   >選択肢はいくつでも追加できます。

   「保存」をクリックします。
   ![](assets/seven.png)

そして、それを持っている！ 個人のパーティションを人で埋めるためのルールを割り当てました！

>[!NOTE]
>
>以前の条件に一致しない場合は、デフォルトの選択が適用されます。

