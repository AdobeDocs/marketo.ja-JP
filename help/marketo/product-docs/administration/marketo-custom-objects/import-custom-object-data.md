---
unique-page-id: 10099680
description: カスタムオブジェクトデータのインポート —Marketoドキュメント — 製品ドキュメント
title: カスタムオブジェクトデータのインポート
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# カスタムオブジェクトデータのインポート {#import-custom-object-data}

カスタムオブジェクトデータをデータベースにインポートするのは簡単です。 会社でカスタムオブジェクトを使用する場合、詳しくは[会社でのカスタムオブジェクトの使用](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies)を参照してください。

1. マイMarketoで、**Database**&#x200B;に移動します。

   ![](assets/db-1.png)

1. 「**新規**」をクリックし、「**カスタムオブジェクトデータを読み込む**」を選択します。

   ![](assets/image2016-4-7-10-6-54.png)

1. 「**参照**」をクリックして、データファイルを探します。 ファイル形式（この例ではコンマ区切り値）を選択します。

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. カスタムオブジェクトを選択します。

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. ドロップダウンから重複除外モードを選択します。 「**次へ**」をクリックします。

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >カスタムオブジェクトレコードを作成または更新する場合は、重複除外フィールドを一意の識別子として使用します。 次の例では、**car**&#x200B;カスタムオブジェクトvin（車両ID番号）のDedupeフィールドを使用しています。 カスタムオブジェクトレコードのみを更新する場合は、「Dedupe Mode」に「MarketoGUID」を選択できます。

1. 各列をMarketoフィールドにマップし、ドロップダウンから選択します。

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >ファイル内の値が、一致するフィールドの種類（テキスト、整数など）と一致することを確認してください。一致しない場合、ファイルは拒否されます。

1. 「**次へ**」をクリックします。

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. 「**インポート**」をクリックします。

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >カスタムオブジェクトのサイズは100 MBが上限です。

   >[!TIP]
   >
   >[**アラートの送信先：**]フィールドに電子メールアドレスを入力すると、インポートが完了した時にMarketoから電子メールが送信されます。

1. 画面の右上隅には、インポートの実行中に通知が表示され、完了時に最終的な結果が表示されます。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   やった！

>[!MORELIKETHIS]
>
>[Marketoのカスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
