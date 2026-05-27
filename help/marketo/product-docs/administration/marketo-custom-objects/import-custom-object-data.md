---
unique-page-id: 10099680
description: カスタムオブジェクトの選択、重複排除モード、フィールドマッピングなど、CSV ファイルを使用してカスタムオブジェクトデータを読み込む手順。
title: カスタムオブジェクトデータのインポート
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
TQID: https://experienceleague.adobe.com/eWVHHONaYWOgc8s6AuB-PpEr-m3G5ixHwf5IondqZKE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 252
ht-degree: 45%

---

# カスタムオブジェクトデータのインポート {#import-custom-object-data}

カスタムオブジェクトデータをデータベースに読み込むには、次の手順に従います。 会社と共にカスタムオブジェクトを使用する場合は、[会社と共にカスタムオブジェクトを使用する](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies)を参照してください。

1. My Marketo で、「**[!UICONTROL データベース]**」に移動します。

   ![](assets/import-custom-object-data-1.png)

1. 「**[!UICONTROL 新規]**」をクリックし、「**[!UICONTROL カスタムオブジェクトデータをインポート]**」を選択します。

   ![](assets/import-custom-object-data-2.png)

1. 「**[!UICONTROL 参照]**」をクリックして、データファイルを探します。 ファイル形式（この例では「コンマ区切り値」）を選択します。

   ![](assets/import-custom-object-data-3.png)

1. [!UICONTROL カスタムオブジェクト]を選択します。

   ![](assets/import-custom-object-data-4.png)

1. ドロップダウンから[!UICONTROL 重複排除モード]を選択します。 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >カスタムオブジェクトレコードを作成または更新する際に、一意のIDとして1つ以上の重複排除フィールドを使用します。 この例では、「**car**」カスタムオブジェクトの重複排除フィールドとして「vin」（車両の ID 番号）を使用します。 カスタムオブジェクトのレコードのみを更新している場合は、[!UICONTROL Marketo Guid] を[!UICONTROL 重複排除モード]として選択できます。

1. ドロップダウンで選択して、各列を Marketo のフィールドにマップします。

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >ファイル内の値が、一致するフィールドのタイプ（テキスト、整数など）と一致していることを確認します。一致しない場合、ファイルは拒否されます。

1. 「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-custom-object-data-7.png)

1. 「**[!UICONTROL 読み込み]**」をクリックします。

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >カスタムオブジェクトのサイズの上限は 100 MB です。

   >[!TIP]
   >
   >「**[!UICONTROL アラートを送信]**」フィールドにメールアドレスを入力すると、インポートが完了するとMarketoからメールが送信されます。

1. 画面の右上隅に、読み込みの実行中に通知が表示され、読み込みが完了すると最終結果が表示されます。

   ![](assets/import-custom-object-data-9.png)

>[!MORELIKETHIS]
>
>[Marketo カスタムオブジェクトについて](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
