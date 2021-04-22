---
unique-page-id: 10093188
description: Marketoのカスタムオブジェクトについて —Marketoドキュメント — 製品ドキュメント
title: Marketoのカスタムオブジェクトについて
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 1%

---

# Marketoのカスタムオブジェクトについて{#understanding-marketo-custom-objects}

カスタムオブジェクトを使用して、ビジネスに固有の指標を追跡します。

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。  詳細は、営業取引先責任者にお問い合わせください。

スマートキャンペーンでは、カスタムオブジェクトをフィルターやトリガーとして使用します。 次に例を示します。

* **フィルタ**:特定の車のブランドの所有者にのみ電子メールを送信
* **トリガー**:カスタムオブジェクトがユーザーまたは会社に追加されたら、電子メールを送信します。

1対多または多対多の関係でカスタムオブジェクトを設定できます。 次に例を示します。

* **1対多**:1人が複数の車を所有している
* **多対多**:複数の学生がコースカタログから複数のコースに登録

1対多の構造体は、単一のリンクフィールドを使用して、カスタムオブジェクトを人または会社に接続します。

多対多カスタムオブジェクトは、中間オブジェクトの一部である2つのリンクフィールドを使用します。 1つのリンクフィールドは個人または会社に接続され、もう1つのリンクフィールドはコースカタログなどのカスタムオブジェクトに接続されます。 この仲介オブジェクトには、コースの等級や出席日など、接続の特性をさらに定義する追加のカスタムフィールドを含めることができます。

>[!TIP]
>
>ユーザーインターフェイス内でカンマ区切り値(CSV)を使用してカスタムオブジェクトを読み込み、データサンプルをテストおよび検証します。 次に、APIを使用してすべてのファイルをアップロードします。

>[!CAUTION]
>
>カスタムオブジェクトは復元できないので、削除する前に必要でないことを確認してください。

## Marketoのカスタムオブジェクトへのアクセス{#accessing-marketo-custom-objects}

1. Marketoのカスタムオブジェクトを作成または編集するには、**管理者**&#x200B;をクリックし、**Marketoカスタムオブジェクト**&#x200B;のリンクをクリックします。

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. Marketoカスタムオブジェクトでは、右側にすべてのカスタムオブジェクトのリストが表示されますが、メイングリッドには承認済みのオブジェクトのみが表示されます。

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. グリッドには、オブジェクト名、レコード数、フィールド数、最新の更新日が表示されます。

   >[!TIP]
   >
   >これらのフィールドは、Marketoによって自動的に更新されますが、[レコード]列のアイコンをクリックすると表示を更新できます。

1. 右側のオブジェクト名をクリックして、詳細ページを開きます。

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## 人に関連付けられた表示カスタムオブジェクト{#view-custom-objects-associated-to-a-person}

カスタムオブジェクト構造の作成後、特定のカスタムオブジェクトデータをアップロードすると、カスタムオブジェクトは、カスタムオブジェクトのリンクフィールドを使用して、データベース内のユーザーに自動的に関連付けられます。 表示情報は、個人の詳細ページの「カスタムオブジェクト」タブから実行できます。

1. **Database**&#x200B;に移動します。

   ![](assets/db.png)

1. データベースを開き、「**ユーザー**」タブをクリックします。 ユーザー設定オブジェクトに関連付けたユーザーのレコードを重複クリックします。

   ![](assets/five.png)

1. 個人の詳細ページで、「**カスタムオブジェクト**」タブをクリックします。 ドロップダウンからオブジェクトを選択します。

   ![](assets/six.png)

1. これで、そのユーザーに関連付けられているそのタイプのすべてのカスタムオブジェクトのリストを表示できます。

   ![](assets/seven.png)

## 会社でのカスタムオブジェクトの使用{#using-custom-objects-with-companies}

会社にリンクされたカスタムオブジェクトは、CRMから会社を同期する場合、またはAPIを使用して明示的に会社を作成する場合に最適です。 また、会社IDをリンクフィールドとして使用することをお勧めします。

Marketoに複数の人がCRMまたはMarketoのみのレコードのレコードを持っている場合、会社にリンクされたカスタムオブジェクトは、複数の個別のレコードに関連付けられません。 これは、会社の下に複数の人がいる場合、会社がCRMから同期された場合、またはAPIを使用して明示的に会社を作成する場合にのみサポートされるからです。

カスタムオブジェクトは、1つのレコードに直接リンクすることのみ可能です。 つまり、カスタムオブジェクトタイプが会社フィールドによってリンクされている場合は、CRMでの連絡先の変換を使用するか、MarketoのREST APIを使用して会社を管理する場合は、externalCompanyIdフィールドを使用して、個人レコードが会社に関連付けられていることを確認します。 会社レコードに明示的にリンクされていない個人レコードの場合、会社を使用してリンクされたカスタムオブジェクトは、会社フィールドの値が多くの人で共有されている場合でも、単一のレコードにランダムにリンクされます。

詳しくは、[カスタムオブジェクトデータの読み込み](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)を参照してください。

>[!MORELIKETHIS]
>
>* [Marketoカスタムオブジェクトの作成](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [カスタムオブジェクトの承認](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Marketoカスタムオブジェクトの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [追加Marketoカスタムオブジェクトフィールド](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Marketoカスタムオブジェクトフィールドの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [カスタムオブジェクトデータのインポート](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

