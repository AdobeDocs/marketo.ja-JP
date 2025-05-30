---
unique-page-id: 10093188
description: Marketo カスタムオブジェクトについて - Marketo ドキュメント - 製品ドキュメント
title: Marketo カスタムオブジェクトについて
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
feature: Custom Objects
source-git-commit: 7fd4d4e12b348ad4d0d69cd3f62cf441eda258b8
workflow-type: ht
source-wordcount: '699'
ht-degree: 100%

---

# Marketo カスタムオブジェクトについて {#understanding-marketo-custom-objects}

自社のビジネスに特有の指標をトラッキングするには、カスタムオブジェクトを使用します。

>[!AVAILABILITY]
>
>すべての Marketo Engage ユーザがこの機能を購入しているわけではありません。詳しくは、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

スマートキャンペーンでは、フィルターおよびトリガーとしてカスタムオブジェクトを使用します。例：

* **フィルター**：特定の自動車ブランドのオーナーにのみメールを送信する
* **トリガー**：カスタムオブジェクトが人または会社に追加されたときにメールを送信する

カスタムオブジェクトは、1 対多または多対多の関係で設定できます。例：

* **1 対多**：1 人の人が複数の自動車を所有している
* **多対多**：複数の学生がコースカタログの複数のコースに登録する

1 対多の構造では、1 つのリンクフィールドを使用してカスタムオブジェクトを人または会社に結び付けます。

多対多のカスタムオブジェクトは、2 つのリンクフィールドと、中間オブジェクトの一部を使用します。一方のリンクフィールドは人または会社に結び付けられ、もう一方はカスタムオブジェクト、例えばコースカタログに結び付けられます。この中間オブジェクトに、さらに他のカスタムフィールド（例えばコースの等級、出席日など）を含め、関係の性質を詳細に定義することができます。

>[!TIP]
>
>データサンプルをテストして検証するには、ユーザーインターフェイスでカンマ区切りの値リスト（CSV）を使用してカスタムオブジェクトをインポートし、API を利用してそのファイルをすべてアップロードします。

>[!CAUTION]
>
>カスタムオブジェクトは復元できないので、削除する前に、本当に不要かどうか確かめてください。

## Marketo カスタムオブジェクトへのアクセス {#accessing-marketo-custom-objects}

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/understanding-marketo-custom-objects-1.png)

1. 「**[!UICONTROL Marketo カスタムオブジェクト]**」をクリックします。

   ![](assets/understanding-marketo-custom-objects-2.png)

1. 「Marketo カスタムオブジェクト」で、右側にカスタムオブジェクトがすべてリストされますが、表示されるのはメイングリッドに公開されたオブジェクトだけです。

   ![](assets/understanding-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >グリッドには、オブジェクト名、レコード数、フィールド数、最新の更新日時が表示されます。

   >[!TIP]
   >
   >各フィールドは自動的に更新されますが、「レコード」列のアイコンをクリックすれば更新できます。

1. 右のオブジェクト名をクリックすると、詳細ページが開きます。

   ![](assets/understanding-marketo-custom-objects-4.png)

## 人物に関連付けられたカスタムオブジェクトの表示 {#view-custom-objects-associated-to-a-person}

カスタムオブジェクト構造を作成しておくと、特定のカスタムオブジェクトデータをアップロードするときに、カスタムオブジェクトがデータベースの人物に自動的に関連付けられます。このとき利用されるのは、カスタムオブジェクトのリンクフィールドです。情報は、人物詳細ページの「[!UICONTROL カスタムオブジェクト]」タブで確認できます。

1. **[!UICONTROL データベース]**&#x200B;に移動します。

   ![](assets/understanding-marketo-custom-objects-5.png)

1. データベースを開き、「**[!UICONTROL 人物]**」タブをクリックします。カスタムオブジェクトに関連付ける人物のレコードをダブルクリックします。

   ![](assets/understanding-marketo-custom-objects-6.png)

1. リード詳細ページで「**[!UICONTROL カスタムオブジェクト]**」タブをクリックし、ドロップダウンからオブジェクトを選択します。

   ![](assets/understanding-marketo-custom-objects-7.png)

1. これで、その人物に関連付けられたタイプのカスタムオブジェクトのすべてがリスト表示されます。

   ![](assets/understanding-marketo-custom-objects-8.png)

   >[!NOTE]
   >
   >人物レコードでは、「カスタムオブジェクト」タブに最大 100 件のレコードを ID の降順に並べ替えて表示できます。

## 企業へのカスタムオブジェクトの使用 {#using-custom-objects-with-companies}

企業にリンクされたカスタムオブジェクトは、CRM から企業を同期する場合、または API を利用して明示的に企業を作成する場合に最もうまく機能します。企業 ID をリンクフィールドとして使用することをお勧めします。

Marketo に複数の人物が設定されていて、それが CRM のレコードまたは Marketo のみのレコードである場合、企業にリンクされているカスタムオブジェクトは、複数の個人レコードには関連付けられません。複数の人物がいる 1 つの企業がサポートされるのは、企業が CRM から同期されるか、API を使用して明示的に企業を作成する場合だけだからです。

カスタムオブジェクトは、1 つのレコードにしか直接リンクできません。つまり、カスタムオブジェクトのタイプが企業フィールドによってリンクされているときには、CRM で連絡先のコンバージョンを使用して、人物レコードを企業に関連付ける必要があるということです。あるいは、Marketo の REST API で企業を管理している場合には、externalCompanyId フィールドを使用して関連付ける必要があります。人物レコードが明示的に企業レコードにリンクされていない場合は、たとえ企業フィールドの値が複数の人によって共有されていても、企業を使用してリンクされているカスタムオブジェクトが 1 つのレコードにリンクされることはまれです。

詳しくは、[カスタムオブジェクトデータのインポート](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)を参照してください。

>[!MORELIKETHIS]
>
>* [Marketo カスタムオブジェクトの作成](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [カスタムオブジェクトの承認](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Marketo カスタムオブジェクトの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Marketo カスタムオブジェクトフィールドの追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Marketo カスタムオブジェクトフィールドの編集と削除](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [カスタムオブジェクトデータのインポート](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)
