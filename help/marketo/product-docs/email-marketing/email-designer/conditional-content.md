---
solution: Marketo Engage
product: marketo
title: 条件付きコンテンツ
description: 条件付きコンテンツをメールで使用すると、受信者に応じたコンテンツを動的に表示できます。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 6f2d3256f3422f1c5054dfd87db3e31c862724a5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 6%

---

# 条件付きコンテンツ {#conditional-content}

条件付きコンテンツを使用すると、オーディエンスに表示するコンテンツを動的に制御できます。 既存のセグメント化を使用して、事前定義された条件に基づいて受信者に表示する内容を決定します。

>[!PREREQUISITES]
>
>少なくとも 1 つのセグメント化 [ 作成 ](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) および [ 承認 ](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md) を持っている。

## 条件付きコンテンツを追加 {#add-conditional-content}

1. 目的のメールを開き、「**メールコンテンツを編集**」をクリックします。

   ![](assets/conditional-content-1.png)

1. 条件付きにするコンテンツを選択します（この例では、ヘッダー画像を選択しています）。 _条件付きコンテンツを有効にする_ アイコンをクリックします。

   ![](assets/conditional-content-2.png)

1. 箱がオレンジ色になります。 左側の _条件を選択_ アイコンをクリックして、バリアントを定義します。

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. 目的のセグメントを選択し、「**選択**」をクリックします。

   ![](assets/conditional-content-4.png)

1. _画像を編集_ アイコンをクリックして、バリアントの既存の画像を置き換えます。 新しい画像のソースを選択します。 この例では、Marketo Engage サブスクリプションで _Images &amp; Files_ ライブラリを選択しています。

   ![](assets/conditional-content-5.png)

1. 該当する画像を選択し、「**選択**」をクリックします。

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. 新しい画像が表示されます。 識別しやすいように、バリアントの名前を変更することをお勧めします。

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. 別のバリアントを追加するには（オプション）、「**バリアントを追加**」をクリックして、同じ手順に従います。

   ![](assets/conditional-content-8.png)

1. 完了したら、各バリアントに選択したコンテンツが表示されます。

   ![](assets/conditional-content-9.gif)

1. 受信者には、各セグメントで定義されたルールに基づいてコンテンツが表示されます。 上の例では、Marketo Engageのフィールド _お気に入りのスポーツ_ に「サッカー」がリストされている人は誰でもサッカーの画像が表示されます。

>[!MORELIKETHIS]
>
>* [セグメントルールの定義](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Marketo でのカスタムフィールドの作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
