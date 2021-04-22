---
unique-page-id: 37355569
description: プログラムメンバのカスタムフィールド —Marketoドキュメント — 製品ドキュメント
title: プログラムメンバのカスタムフィールド
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 1%

---

# プログラムメンバのカスタムフィールド{#program-member-custom-fields}

プログラムメンバのカスタムフィールドを使用すると、各メンバのプログラム固有のデータを収集できます。 これらは、次の場所で使用できます。Marketoフォーム、スマートリストフィルターおよびトリガー、スマートキャンペーンフローアクション。 データは、プログラムの「メンバー」タブで表示できます。

>[!NOTE]
>
>現時点では、プログラムメンバのカスタムフィールドは、Salesforceキャンペーンメンバのフィールドとの統合を備えていません。

## プログラムメンバのカスタムフィールドの作成{#create-a-program-member-custom-field}

1. Marketoで、**管理者**&#x200B;をクリックします。

   ![](assets/one.png)

1. 「**フィールド管理**」をクリックします。

   ![](assets/two.png)

1. 「**新しいカスタムフィールド**」をクリックします。

   ![](assets/three.png)

1. 「オブジェクト」ドロップダウンをクリックし、目的のオブジェクトを選択します。

   ![](assets/four.png)

   >[!NOTE]
   >
   >[個人]と[プログラムメンバ]のカスタムフィールドは、同じ名前を共有できません。

1. 残りのフィールドに入力し、「**作成**」をクリックします。

   ![](assets/five.png)

   >[!NOTE]
   >
   >プログラムメンバのカスタムフィールドでサポートされる型は次のとおりです。boolean、date、datetime、float、integer、string、URL。 [フィールドの種類の詳細を表示します](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md)。

## オブジェクトの説明{#object-descriptions}

| オブジェクト | 詳細 |
|---|---|
| 企業 | 個人に関連付けられている会社の名前。 |
| 商談 | オポチュニティは、将来の潜在的なセールとして個人またはアカウントに関連付けることができます。 通常、CRM経由またはAPI経由でMarketoに入ります。 |
| 担当者 | マーケティングキャンペーンを通じて関与しているMarketoデータベースの個人。 |
| プログラムメンバー | プログラムの一員である者 |

## トリガーとフィルター{#triggers-and-filters}

[トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)や[フィルター](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)を介して、スマートリストでこのプログラム固有のデータを活用できます。

![](assets/six.png)

## {#things-to-know}の知り合い

* プログラムメンバーのカスタムフィールドは、ローカルアセットでのみ使用できます。 特定のプログラムに関連付ける方法がないので、Design Studioではサポートされません。
* プログラムメンバーカスタムフィールドを含むフォーム(またはフォームを含むランディングページ)をDesign Studioにコピーまたは移動することはできません。
* プログラムメンバオブジェクトには、最大20個のカスタムフィールドを含めることができます。 これらのフィールドは、どのプログラムでも使用できます。
* プログラムのメンバを削除すると、そのユーザの[プログラムメンバ]カスタムフィールドにデータがある場合、そのフィールドからデータがスクラブされます。
* データを表示するには、プログラムの「Members」タブをクリックし、該当するフィールドを含むカスタム表示を作成します。
* [リスト](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)と[API](https://developers.marketo.com/)を介した読み込みと書き出しがサポートされています。
* 2人のユーザーを結合すると、推奨結果のプログラムメンバーのカスタムフィールドデータが使用されます。 ただし、勝者に何もない場合は、敗者の値が使用されます。

>[!MORELIKETHIS]
>
>[Marketoでカスタムフィールドを作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
