---
unique-page-id: 10097613
description: Marketo カスタムオブジェクトリンクフィールドの追加 - Marketo ドキュメント - 製品ドキュメント
title: Marketo カスタムオブジェクトリンクフィールドの追加
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 1dbe820e126f92ce5820e38414925605372a4b09
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 85%

---

# Marketo カスタムオブジェクトリンクフィールドの追加 {#add-marketo-custom-object-link-fields}

カスタムオブジェクトを作成する場合は、カスタムオブジェクトレコードを正しい親レコードに接続するためのリンクフィールドを指定する必要があります。

* 1 対多のカスタム構造の場合は、カスタムオブジェクトのリンクフィールドを使用して、カスタム構造を個人または会社に接続します。
* 多対多構造の場合は、2 つのリンクフィールドを使用し、別に作成した中間オブジェクト（カスタムオブジェクトの一種でもある）から接続します。1 つのリンクはデータベース内の人や会社に接続し、もう 1 つのリンクはカスタムオブジェクトに接続します。この場合、リンクフィールドはカスタムオブジェクト自体に配置されません。

>[!IMPORTANT]
>
>Marketo Engageは、[ 多対多 ] 関係の各ブリッジオブジェクトに対して 1 つのエッジオブジェクトのみをサポートします。 以下のサンプルでは、各登録者は 1 つのコースにのみリンクできます。 ただし、各コースには学生登録が多い（多対 1 の関係）のと同様に、各エッジオブジェクトには多数のブリッジオブジェクトが存在する場合があります。 Bridge オブジェクトレコード（1 対多または多対多）に対して複数の Edge オブジェクトレコードが存在するようにカスタムオブジェクトデータが構造化されている場合、それぞれが 1 つの Edge オブジェクトレコードを参照する複数の Bridge オブジェクトレコードをMarketoで作成できます。

## 1 対多構造のリンクフィールドの作成 {#create-a-link-field-for-a-one-to-many-structure}

以下に、1 対多の構造のカスタムオブジェクトにリンクフィールドを作成する方法を示します。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. 「**[!UICONTROL Marketo カスタムオブジェクト]**」をクリックします。

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. リストからカスタムオブジェクトを選択します。

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. 「**[!UICONTROL フィールド]**」タブで、「**[!UICONTROL 新規フィールド]**」をクリックします。

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. リンクフィールドに名前を付けて、オプションで[!UICONTROL 説明]を追加します。必ず「[!UICONTROL リンク]」データタイプを選択してください。

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >カスタムオブジェクトが承認されると、[!UICONTROL リンク]フィールドや[!UICONTROL 重複排除フィールド]の作成、編集、削除に戻ることはできません。

1. [!UICONTROL リンクオブジェクト]の対象が[!UICONTROL リード]（人物）か[!UICONTROL 会社]かを選択します。

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >「[!UICONTROL リード]」を選択すると、ID、メールアドレスおよびカスタムフィールドがリストに表示されます。
   >
   >「[!UICONTROL 会社]」を選択すると、ID およびカスタムフィールドがリストに表示されます。

1. 新しいフィールドの親として接続する[!UICONTROL リンクフィールド]を選択します。

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >リンクフィールドでは、文字列フィールドタイプのみがサポートされています。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## 多対多構造のリンクフィールドの作成 {#create-a-link-field-for-a-many-to-many-structure}

以下に、多対多構造で使用するリンクフィールドを中間オブジェクトに作成する方法を示します。

>[!PREREQUISITES]
>
>既に中間オブジェクトと、その中間オブジェクトをリンクするカスタムオブジェクトを作成している必要があります。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. 「**[!UICONTROL Marketo カスタムオブジェクト]**」をクリックします。

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. フィールドを追加する中間オブジェクトを選択します。

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. 「**[!UICONTROL フィールド]**」タブで、「**[!UICONTROL 新規フィールド]**」をクリックします。

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. 2 つのリンクフィールドを作成する必要があります。一度に 1 つずつ作成します。まず、データベースリストのメンバーのフィールドに名前を付けます（例：leadID）。オプションで[!UICONTROL 説明]を追加します。必ず「[!UICONTROL リンク]」[!UICONTROL データタイプ]を選択してください。

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >カスタムオブジェクトが承認されると、[!UICONTROL リンク]フィールドや[!UICONTROL 重複排除フィールド]の作成、編集、削除に戻ることはできません。

1. データベースから[!UICONTROL リンクオブジェクト]（この場合は「[!UICONTROL リード]」）を選択します。

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. 接続する[!UICONTROL リンクフィールド]（この場合は [!UICONTROL ID]）を選択します。

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >[!UICONTROL リンクフィールド]では、文字列フィールドタイプのみがサポートされています。

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. カスタムオブジェクトへの 2 番目のリンク（この例では courseID）に対して、この手順を繰り返します。「[!UICONTROL リンクオブジェクト]」名は「コース」、「[!UICONTROL リンクフィールド]」は「courseID」になります。既にコースのカスタムオブジェクトを作成し承認しているので、これらの選択はドロップダウンメニューで使用できます。

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. 「enrollmentID」や「成績」など、中間オブジェクトで使用するその他のフィールドを作成します。

## カスタムオブジェクトの使用 {#using-custom-objects}

次の手順では、スマートキャンペーンのフィルターでこれらのカスタムオブジェクトを使用します。多対多の関係では、複数の人／会社および複数のカスタムオブジェクトを選択できます。以下の例では、データベース内でこれらの条件に一致する人がすべて表示されます。「コース名」フィールドはコースカスタムオブジェクトから、「登録成績」は中間オブジェクトから取得されます。

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Marketo カスタムオブジェクトフィールドの追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Marketo カスタムオブジェクトの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Marketo カスタムオブジェクトフィールドの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
