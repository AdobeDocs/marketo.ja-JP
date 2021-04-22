---
unique-page-id: 10093688
description: 追加Marketoカスタムオブジェクトフィールド —Marketoドキュメント — 製品ドキュメント
title: 追加Marketoカスタムオブジェクトフィールド
translation-type: tm+mt
source-git-commit: 65182770291dc14fbe915a40403fc09b433aae86
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# 追加Marketoカスタムオブジェクトフィールド{#add-marketo-custom-object-fields}

カスタムオブジェクトを作成したら、ビジネスニーズに合わせてフィールドを追加する必要があります。

フィールドは、カスタムオブジェクトで使用される特定の情報を定義します。 リンクフィールドは、カスタムオブジェクトを接続する特別な役割を持ち、[個別の記事](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)で扱われます。

1. 「**管理者**」をクリックし、**データベース管理**&#x200B;で「**Marketoカスタムオブジェクト**」を選択します。

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. 右側のフィールドの追加先のオブジェクトを選択します。

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. 「**フィールド**」タブで、「**新しいフィールド**」をクリックします。

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >上記の3つのフィールドは、カスタムオブジェクトを作成するときに、Marketoによって自動的に作成されます。 これらのフィールドは、Marketoが自動的に管理するので、編集や削除はできません。

1. 表示名と説明を入力します。

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >API名は、承認されるまで編集できません。

1. 次に、リストから適切なデータタイプを選択します。

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. 新しいフィールドを一意の識別子として使用する場合は、重複除外スライダを引っ張ります。 「**保存**」をクリックして終了します。

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >重複除外フィールドは、カスタムオブジェクトの取得、更新、削除に使用できます。 すべてのカスタムオブジェクト定義には、重複除外フィールドを少なくとも1つ（3つ以内）含める必要があります。

1. 必要な追加その他のフィールド。

   >[!NOTE]
   >
   >1対多の構造を作成する場合は、カスタムオブジェクトにリンクフィールドを追加する必要があります。 多対多の構造の場合、カスタムオブジェクトにリンクフィールドは必要ありませんが、中間オブジェクトに2つのリンクフィールドを追加する必要があります。 リンクフィールドを作成するには、[Marketoカスタムオブジェクトリンクフィールド](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)を参照してください。カスタムオブジェクトの種類の詳細については、[Marketoカスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)を参照してください。

>[!MORELIKETHIS]
>
>* [追加Marketoカスタムオブジェクトリンクフィールド](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Marketoカスタムオブジェクトの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Marketoカスタムオブジェクトフィールドの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Marketoのカスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

