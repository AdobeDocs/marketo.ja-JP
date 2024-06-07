---
unique-page-id: 2949962
description: フォームフィールドの表示設定の動的な切り替え - Marketo ドキュメント - 製品ドキュメント
title: フォームフィールドの表示設定の動的な切り替え
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 99%

---

# フォームフィールドの表示設定の動的な切り替え {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [フォームへの国選択リストの追加](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Marketo フォームの素晴らしい機能の 1 つは、フォームフィールドや[フィールドセット](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md)の表示設定を動的に切り替えられることです。

>[!NOTE]
>
>**例**
>
>この例では、**国**&#x200B;が「米国」として選択されていない限り、「**州**」フィールドを非表示にします。

1. 「**マーケティングアクティビティ**」に移動します。

   ![](assets/login-marketing-activities-8.png)

1. フォームを選択し、「**フォームの編集**」をクリックします。

   ![](assets/editform-1.png)

1. 表示設定を動的に切り替えるフィールドを選択し、「**表示設定ルール**」リンクをクリックします。

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 条件として指定するフィールドを検索して選択します。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 演算子を選択します。

   >[!TIP]
   >
   >「次の語句で始まる」のようなあいまい一致を選択できるので、これは素晴らしいです。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 検索する値を選択し、ドロップダウンの外側をクリックします。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >ドロップダウンを開いた状態で複数の値をクリックして選択できます。例えば、「米国」と「カナダ」を選択できます。

   >[!NOTE]
   >
   >既に、「国」のフィールドタイプを候補リストに変換し、[すべての国を値として追加する](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)作業を完了しているものとします。

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-15-15-3a18-3a15.png)

これで手順は完了です。訪問者がこのフィールドに入力し、「国」で「米国」を選択すると、選択肢が指定された状態で「州」フィールドが動的に表示されます。

>[!IMPORTANT]
>
>Forms 2.0 の [API 関数](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"}カスタムスクリプトを使用してフィールド値が設定または更新された場合、フォームフィールドの動作はシームレスに機能します。
>
>Forms 2.0 JavaScript API 以外の外部スクリプトでフィールドの値が変更されると、条件付きフィールドが期待どおりに動作しない場合があります。
