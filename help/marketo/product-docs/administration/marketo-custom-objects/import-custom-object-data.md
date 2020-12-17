---
unique-page-id: 10099680
description: カスタムオブジェクトデータのインポート — Marketto Docs — 製品ドキュメント
title: カスタムオブジェクトデータの読み込み
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# カスタムオブジェクトデータの読み込み{#import-custom-object-data}

カスタムオブジェクトデータをデータベースにインポートするのは簡単です。 会社でカスタムオブジェクトを使用する場合、詳しくは[会社でのカスタムオブジェクトの使用](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies)を参照してください。

1. 「My Marketo」で、**Database**&#x200B;に移動します。

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
   >カスタムオブジェクトレコードを作成または更新する場合は、重複除外フィールドを一意の識別子として使用します。 次の例では、**car**&#x200B;カスタムオブジェクトvin（車両ID番号）のDedupeフィールドを使用しています。 カスタムオブジェクトレコードのみを更新する場合は、重複除外モードとしてMarketo Guidを選択できます。

1. 各列を「マーケティング先」フィールドにマップし、ドロップダウンから選択します。

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
   >「**アラートの送信先：**」フィールドに電子メールアドレスを入力すると、インポートが完了したら、Marketorから電子メールが送信されます。

1. 画面の右上隅には、インポートの実行中に通知が表示され、完了時に最終的な結果が表示されます。

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   やった！

>[!MORELIKETHIS]
>
>* [マーケティングカスタムオブジェクトについて](understanding-marketo-custom-objects.md)

>



