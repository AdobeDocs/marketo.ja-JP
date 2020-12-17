---
unique-page-id: 2949962
description: フォームフィールドの表示/非表示を動的に切り替える — Marketto Docs — 製品ドキュメント
title: フォームフィールドの表示/非表示を動的に切り替える
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---


# フォームフィールドの表示/非表示を動的に切り替える{#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [フ追加ォームの国選択リスト](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



Marketoフォームの非常に優れた機能の1つは、フォームフィールドまたは[フィールドセット](add-a-fieldset-to-a-form.md)を動的に非表示/表示できる点です。

>[!NOTE]
>
>**例**
>
>この例では、「**国**」が「米国」として選択されていない限り、「**州**」フィールドを非表示にします。

1. **マーケティング** **アクティビティ**&#x200B;に移動します。

   ![](assets/login-marketing-activities-8.png)

1. フォームを選択し、「**編集** **フォーム**」をクリックします。

   ![](assets/editform-1.png)

1. 動的に表示/非表示にするフィールドを選択し、**表示****ルール**&#x200B;のリンクをクリックします。

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. 条件を作成するフィールドを探して選択します。

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. 演算子を選択します。

   >[!TIP]
   >
   >「開始」のようなあいまいなマッチを選ぶので、これは格好いいです。

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. 検索する値を選択し、ドロップダウンの外側をクリックします。

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >ドロップダウンを開いているときに複数の値をクリックすると、複数の値を選択できます。 例えば、「United States」と「Canada」を選択できます。

   >[!NOTE]
   >
   >以前は、「国」を「ピックリスト」フィールドタイプに変換し、[すべての国を値](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)として追加していました。

1. 「**保存**」をクリックします。

   ![](assets/image2014-9-15-15-3a18-3a15.png)

それだ！ 現在は、ユーザーがこのフォームに入力し、「国別」で「米国」を選択すると、指定した選択肢と共に「州」フィールドが動的に表示されます。

>[!NOTE]
>
>**ディープダイブ**
>
>[フォーム](http://docs.marketo.com/display/docs/forms)の詳細を知りたい場合は、

