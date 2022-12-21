---
unique-page-id: 10093192
description: Marketo カスタムオブジェクトの作成 - Marketo ドキュメント - 製品ドキュメント
title: Marketo カスタムオブジェクトの作成
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 100%

---

# Marketo カスタムオブジェクトの作成 {#create-marketo-custom-objects}

自社のビジネスに固有の指標をトラックするには、Marketo カスタムオブジェクトを使用します。カスタムオブジェクトは、自動車、コースなど、Marketo でキャンペーンを実行するためにモデル化するものなら何でも可能です。

>[!NOTE]
>
>1 対多または多対多で動作するカスタムオブジェクトを設定できます。最初のオブジェクトも同じ方法で作成しますが、オブジェクトへのフィールドの追加を開始する際の手順は異なります。詳しくは、[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)を参照してください。

>[!NOTE]
>
>カスタムオブジェクトが承認されると、リンクまたは重複排除フィールドの作成、編集、削除はできなくなります。

## 1 対多構造のカスタムフィールドの作成 {#create-a-custom-object-for-a-one-to-many-structure}

この例では、1 対多の構造で使用する「自動車」カスタムオブジェクトを示します。後で、多対多構造で使用する「コース」カスタムオブジェクトと中間オブジェクトを作成します。

1. 「**管理者**」をクリックし「**データベース管理**」で「**Marketo カスタムオブジェクト**」を選択します。

   ![](assets/image2016-1-18-13-3a12-3a19.png)

1. 「**新規カスタムオブジェクト**」をクリックします。

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >「Marketo カスタムオブジェクト」タブには、右側にすべてのカスタムオブジェクトと、最新の更新時のレコード数とフィールド数を含む、承認済みオブジェクトの詳細が表示されます。

1. 表示名を入力します。「API 名」と「複数名」は自動的に入力されます。説明を入力します（オプション）。

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >これらのフィールドは、作成時に編集できますが、保存後は、「複数名」フィールドと「**リード詳細で表示**」スライダーのみ編集できます。

1. リードデータベースページにカスタムオブジェクトデータを表示する場合、「**リード詳細で表示**」スライダーを引いて、「**表示**」を表示します。「**保存**」をクリックします。

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. カスタムオブジェクト情報には、入力した内容が表示されます。ステートがドラフトであることに注意してください。

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   次の手順は、フィールドを追加して、[カスタムオブジェクトを作成](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)します。

   >[!NOTE]
   >
   >Marketo カスタムオブジェクトの入力は、リストのインポート、すなわち [API](https://developers.marketo.com/documentation/rest/) 経由でのみ可能です。

## 多対多構造のカスタムフィールドの作成 {#create-a-custom-object-for-a-many-to-many-structure}

この例では、「コース」のカスタムオブジェクトを示します。このオブジェクトを使用して、人物／会社とコースの間に多対多の関係を作成します。作業が完了したら、中間オブジェクトを作成して、データベース内の人物や会社に接続します。

>[!NOTE]
>
>多対多の関係の場合、カスタムオブジェクト内にリンクを作成する必要はありません。代わりに、中間オブジェクトに 2 つのリンクを追加します（以下を参照）。

1. 「**管理者**」をクリックし「**データベース管理**」で「**Marketo カスタムオブジェクト**」を選択します。

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. 「**新規カスタムオブジェクト**」をクリックします。

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. 表示名を入力します。「API 名」と「複数名」は自動的に入力されます。説明を入力します（オプション）。

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >これらのフィールドは、作成時に編集できますが、保存後は、「複数名」フィールドと「**リード詳細で表示**」スライダーのみ編集できます。

1. リードデータベースページにカスタムオブジェクトデータを表示する場合、「**リード詳細で表示**」スライダーを引いて、「**表示**」を表示します。「**保存**」をクリックします。

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. カスタムオブジェクト情報には、入力した内容が表示されます。ステートがドラフトであることに注意してください。

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Marketo カスタムオブジェクトの入力は、リストのインポート、すなわち [API](https://developers.marketo.com/documentation/rest/) 経由でのみ可能です。

次の手順は、中間オブジェクトを作成します（以下を参照）。ただし、その前に、リンク先のフィールドを作成する必要があります。

## 中間オブジェクトの作成 {#create-an-intermediary-object}

カスタムオブジェクトを人物や会社に接続するには、中間オブジェクトを使用します。この例では、「コース」カスタムオブジェクト内のコースをデータベース内の人物や会社に接続するために使用します。

>[!NOTE]
>
>1 対多のカスタムオブジェクト構造の中間オブジェクトを作成する必要はありません。

1. 「**管理者**」をクリックし、「**データベース管理**」で「**Marketo カスタムオブジェクト**」を選択します。

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. 「**新規カスタムオブジェクト**」をクリックします。

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. 表示名を入力します。「API 名」と「複数名」は自動的に入力されます。説明を入力します（オプション）。

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >これらのフィールドは、作成時に編集できますが、保存後は、「複数名」フィールドと「リード詳細で表示」スライダーのみ編集できます。

1. リードデータベースページにカスタムオブジェクトデータを表示する場合、「**リード詳細で表示**」スライダーを引いて、「**表示**」を表示します。「**保存**」をクリックします。

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. カスタムオブジェクト情報には、入力した内容が表示されます。ステートがドラフトであることに注意してください。

   次の手順は、[リンクフィールドを追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)して、中間オブジェクトを人物／会社とカスタムオブジェクトに接続します。

>[!MORELIKETHIS]
>
>* [Marketo カスタムオブジェクトフィールドの追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Marketo カスタムオブジェクトリンクフィールドの追加](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

