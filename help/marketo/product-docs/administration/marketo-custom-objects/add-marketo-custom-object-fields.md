---
unique-page-id: 10093688
description: 表示名、説明、データタイプなど、カスタムオブジェクトにフィールドを追加する手順。
title: Marketo カスタムオブジェクトフィールドの追加
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 40d7e8a0723946970c49a6dfc4f0de4c71b0df65
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 57%

---

# Marketo カスタムオブジェクトフィールドの追加 {#add-marketo-custom-object-fields}

カスタムオブジェクトを作成したら、ビジネスニーズに合わせてフィールドを追加する必要があります。

フィールドでは、カスタムオブジェクトによって使用される特定の情報が定義されます。 リンクフィールドは、特定の目的（カスタムオブジェクトの接続）を果たします。詳しくは、[別の記事](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)を参照してください。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-marketo-custom-object-fields-1.png)

1. 「**[!UICONTROL Marketo カスタムオブジェクト]**」をクリックします。

   ![](assets/add-marketo-custom-object-fields-2.png)

1. 右側でフィールドを追加するオブジェクトを選択します。

   ![](assets/add-marketo-custom-object-fields-3.png)

1. 「**[!UICONTROL フィールド]**」タブをクリックして、「**[!UICONTROL 新規フィールド]**」をクリックします。

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >上記の 3 つのフィールドは、カスタムオブジェクトの作成時に Marketo によって自動的に作成されます。 Marketoはこれらのフィールドを自動的に管理するため、編集や削除はできません。

1. [!UICONTROL 表示名]と（オプションで）[!UICONTROL 説明]を入力します。

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >[!UICONTROL API名]は、承認されるまで編集できます。

1. リストから適切な[!UICONTROL &#x200B; データタイプ &#x200B;]を選択します。

   ![](assets/add-marketo-custom-object-fields-6.png)

1. 新しいフィールドを一意の識別子として使用する場合は、[!UICONTROL 重複排除]スライダーをオンにします。 「**[!UICONTROL 保存]**」をクリックして終了します。

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >重複排除フィールドは、カスタムオブジェクトの取得、更新、削除に使用できます。 すべてのカスタムオブジェクト定義には、重複排除フィールドを少なくとも 1 つ含める必要があります（3 つまで）。

1. 必要なその他のフィールドを追加します。

   >[!NOTE]
   >
   >1対多の構造を構築する場合は、カスタムオブジェクトにリンクフィールドを追加する必要があります。 多対多の構造の場合、カスタムオブジェクトにリンクフィールドは必要ありませんが、中間オブジェクトに2つのリンクフィールドを追加する必要があります。 Marketo カスタムオブジェクトのタイプについて詳しくは、[カスタムオブジェクトリンクフィールドの追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)を参照してリンクフィールドを作成し、[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)を参照してください。

>[!MORELIKETHIS]
>
>* [Marketo カスタムオブジェクトリンクフィールドの追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Marketo カスタムオブジェクトの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Marketo カスタムオブジェクトフィールドの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
