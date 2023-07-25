---
unique-page-id: 10099680
description: カスタムオブジェクトデータのインポート - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクトデータのインポート
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 78%

---

# カスタムオブジェクトデータのインポート {#import-custom-object-data}

カスタムオブジェクトデータをデータベースに簡単にインポートすることができます。会社でカスタムオブジェクトを使用する場合、詳しくは、[会社でカスタムオブジェクトを使用する](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies)を参照してください。

1. My Marketo で、「**[!UICONTROL データベース]**」に移動します。

   ![](assets/import-custom-object-data-1.png)

1. 「**[!UICONTROL 新規]**」をクリックし、「**[!UICONTROL カスタムオブジェクトデータをインポート]**」を選択します。

   ![](assets/import-custom-object-data-2.png)

1. 「**[!UICONTROL 参照]**」をクリックして、データファイルを探します。ファイル形式（この例では「コンマ区切り値」）を選択します。

   ![](assets/import-custom-object-data-3.png)

1. を選択します。 [!UICONTROL カスタムオブジェクト].

   ![](assets/import-custom-object-data-4.png)

1. を選択します。 [!UICONTROL デデュープモード] 」をクリックします。 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >カスタムオブジェクトレコードを作成または更新する際に、重複排除フィールドを一意の識別子として使用します。この例では、「**car**」カスタムオブジェクトの重複排除フィールドとして「vin」（車両の ID 番号）を使用します。カスタムオブジェクトレコードのみを更新する場合は、 [!UICONTROL Marketo Guid] を [!UICONTROL デデュープモード].

1. ドロップダウンで選択して、各列を Marketo のフィールドにマップします。

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >ファイル内の値が、照合先のフィールドのタイプ（テキスト、整数など）と一致することを確認してください。一致しない場合、ファイルは拒否されます。

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-custom-object-data-7.png)

1. 「**[!UICONTROL インポート]**」をクリックします。

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >カスタムオブジェクトのサイズの上限は 100 MB です。

   >[!TIP]
   >
   >電子メールアドレスを **[!UICONTROL アラートの送信先]** フィールドとMarketoは、インポートが完了すると電子メールで送信されます。

1. 画面の右上隅に、インポート実行中には通知が表示され、完了すると最終結果が表示されます。

   ![](assets/import-custom-object-data-9.png)

   これで完了です。

>[!MORELIKETHIS]
>
>[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
