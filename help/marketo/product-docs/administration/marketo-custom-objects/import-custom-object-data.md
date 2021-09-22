---
unique-page-id: 10099680
description: カスタムオブジェクトデータのインポート - Marketo ドキュメント - 製品ドキュメント
title: カスタムオブジェクトデータのインポート
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '233'
ht-degree: 100%

---

# カスタムオブジェクトデータのインポート {#import-custom-object-data}

カスタムオブジェクトデータをデータベースに簡単にインポートすることができます。会社でカスタムオブジェクトを使用する場合、詳しくは、[会社でカスタムオブジェクトを使用する](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies)を参照してください。

1. My Marketo で、「**データベース**」に移動します。

   ![](assets/db-1.png)

1. 「**新規**」をクリックし、「**カスタムオブジェクトデータをインポート**」を選択します。

   ![](assets/image2016-4-7-10-6-54.png)

1. 「**参照**」をクリックして、データファイルを探します。ファイル形式（この例では「コンマ区切り値」）を選択します。

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. カスタムオブジェクトを選択します。

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. ドロップダウンから「重複排除モード」を選択します。「**次へ**」をクリックします。

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >カスタムオブジェクトレコードを作成または更新する際に、重複排除フィールドを一意の識別子として使用します。この例では、「**car**」カスタムオブジェクトの重複排除フィールドとして「vin」（車両の ID 番号）を使用します。カスタムオブジェクトのレコードを更新するだけの場合は、重複排除モードとして「Marketo Guid」を選択できます。

1. ドロップダウンで選択して、各列を Marketo のフィールドにマップします。

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >ファイル内の値が、照合先のフィールドのタイプ（テキスト、整数など）と一致することを確認してください。一致しない場合、ファイルは拒否されます。

1. 「**次へ**」をクリックします。

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >カスタムオブジェクトのサイズの上限は 100 MB です。

   >[!TIP]
   >
   >「**アラートの送信先**」にメールアドレスを入力すると、インポートの完了時にメールが届きます。

1. 画面の右上隅に、インポート実行中には通知が表示され、完了すると最終結果が表示されます。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   これで完了です。

>[!MORELIKETHIS]
>
>[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
