---
unique-page-id: 2359418
description: 人物のリストの読み込み — Marketto Docs — 製品ドキュメント
title: 人物のリストのインポート
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# ユーザーのリストのインポート{#import-a-list-of-people}

## ミッション：トレードショーの出席者のスプレッドシートリストをデータベースにインポートします{#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[設定と追加人](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

このチュートリアルでは、スプレッドシートファイルからMarketoに人をインポートする方法を学びます。

## 手順1:スプレッドシートのダウンロードと編集{#step-download-and-edit-a-spreadsheet}

1. 開始するには、練習用のスプレッドシートファイル([**tradeshow-attendees.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv))をお使いのコンピューターにダウンロードしてください。

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >日付をインポートする場合は、次の形式を使用します。**9/21/20** （月/日/年）

   >[!NOTE]
   >
   >読み込まれる日付/時間フィールドは、すべて中央時間として扱われます。 別のタイムゾーンに日付/時間フィールドがある場合、Excelの数式を使用して中央標準時（米国/シカゴ）に変換できます。

1. 名追加、姓、電子メールアドレス、肩書きを自分のコンピュータに保存します。

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>CSVファイルに実際の電子メールアドレスを入力して、次のミッションで送信する育成用の電子メールを受け取れるようにします。

## 手順2:プログラムの作成{#step-create-a-program}

1. **マーケティングアクティビティ**&#x200B;エリアに移動します。

   ![](assets/ma-2.png)

1. **学習**&#x200B;フォルダーを選択し、**新しい**&#x200B;の下にある&#x200B;**新しいプログラム**&#x200B;をクリックします。

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **「My Tradeshowプログラム」というプログラム名を付け、「** プログラムタイプ ****」で「イベント」を選択します。

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. **チャネル**&#x200B;に対してトレードショー&#x200B;**を選択し、**&#x200B;作成&#x200B;**をクリックします。**

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>イベントプログラムは特定の日付に発生します。 [**イベント**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md)&#x200B;の詳細。

## 手順3:スプレッドシートをMarketorにインポート{#step-import-your-spreadsheet-into-marketo}

1. **マイトレードショープログラム**&#x200B;で、**新規**&#x200B;をクリックし、**新規ローカルアセット**&#x200B;を選択します。

   ![](assets/seven-3.png)

1. **リスト**&#x200B;をクリックします。

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **リストに「Tradeshow Attendees」という名前を付け、「** 作成 ****」をクリックします。

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. **出席者のトレードショー**&#x200B;リストで、**リストアクション**&#x200B;をクリックし、**リストの読み込み**&#x200B;を選択します。

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >独自のCSVファイルを使用する場合は、エンコードがUTF-8、UTF-16、Shift-JISまたはEUC-JPであることを確認してください。

   >[!NOTE]
   >
   >CSVファイルのサイズの上限は100 MBです。

1. **コンピューター上の** tradeshow-attendees. **csvspreadsheetファイルを参照し、「** 次へ ****」をクリックします。

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >リストインポートモードで、「**新しい人をスキップして更新**」を選択すると、既存の人のレコードに影響を与えず、アクティビティを記録しません。 マーケティングアクティビティで使用する既存のユーザーを、事前にフィルタリングされた迅速な静的リストにしたい場合に、このモードを使用します。 このモードを選択すると、次の操作が行われます。
   >
   > * 新しい人物の作成をスキップ
   > * 個人フィールドの更新をスキップ
   > * アクティビティログをスキップ


1. リスト列のフィールドを対応するマーケティング先フィールドにマップし、**次へ**&#x200B;をクリックします。

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >最適な自動マッピングの結果を得るには、列見出しは常にフィールドと完全に一致する（大文字と小文字が区別されます）必要があります。 カスタムフィールドを使用していて、ドロップダウンに表示されない場合は、前のページに戻って[作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)し、オプションにすることができるようにします。

   >[!NOTE]
   >
   >インポートしないフィールドがある場合は、「マーケティング先フィールド」ドロップダウンメニューで「**無視**」を選択します。

1. ****&#x200B;獲得プログラム&#x200B;**に対して「マイトレードショープログラム**」を選択し、**インポート**&#x200B;をクリックします。

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. ユーザーがインポートするのを待ってから、インポートの進行状況ポップアップを閉じます。

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. **マイトレードショープログラム**&#x200B;に戻り、**メンバー**&#x200B;タブをクリックします。 読み込んだユーザーがすべて表示されます。

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>プログラムのメンバーシップを追跡することで、プログラムの成功を分析できます。 [**プログラム**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)&#x200B;の詳細。

## ミッション完了{#mission-complete}

トレードショーの出席者は、Marketoプログラムのメンバーになりました。

<br> 

[エスケアミッション4:電子メールの自動応答](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[ミッション6:ドリップ、ドリップ、Nurture §](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
