---
unique-page-id: 2359418
description: 人物のリストのインポート - Marketo ドキュメント - 製品ドキュメント
title: 人物のリストのインポート
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 100%

---

# 人物のリストのインポート {#import-a-list-of-people}

## ミッション：トレードショーの出席者のスプレッドシートリストをデータベースに読み込む {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[セットアップと人物の追加](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

このチュートリアルでは、スプレッドシートファイルから Marketo に人物を読み込む方法を学びます。

## 手順 1：スプレッドシートをダウンロード／編集する {#step-download-and-edit-a-spreadsheet}

1. まず、練習用のスプレッドシートファイル（[**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}）を PC にダウンロードしてください。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >日付を読み込む場合は、以下の形式を使用します。**9/21/20**（月/日/年）。

   >[!NOTE]
   >
   >読み込まれる日時フィールドは、すべて米中央時間として扱われます。日時フィールドのタイムゾーンが異なる場合、Excel の数式を使用して、中央時刻（米国／シカゴ）に変換できます。

1. 自分の姓、名、実際のメールアドレス（次のミッションで送信するメールを受け取れるように）、役職を追加します。ファイルをコンピューターに保存します。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* メールアドレスには、ASCII 文字のみを含める必要があります。
   >
   >* Marketo は、絵文字を含むメールアドレスを&#x200B;**サポートしていません**。
   >
   >* CSV 経由で `NULL` 値を読み込むと、_フィールドが既に空白であっても_、人物の[アクティビティログ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}の数値フィールドに「データ値を変更」が生成される可能性があります。「データ値の変更」フィルターまたは「データ値の変更」トリガーを使用する[スマートキャンペーン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"}がある場合、データが実際には変更されていない場合でも、人物がこれらのキャンペーンに該当する可能性があります。[制約](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}を使用すると、読み込み時に誰もこれらのキャンペーンに該当しないようにすることができます。

## 手順 2：プログラムを作成する {#step-create-a-program}

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;領域に移動します。

   ![](assets/import-a-list-of-people-3.png)

1. **学習**&#x200B;フォルダーを選択し、「**[!UICONTROL 新規]**」で「**[!UICONTROL 新規プログラム]**」をクリックします。

   ![](assets/import-a-list-of-people-4.png)

1. プログラムに「トレードショープログラム」と&#x200B;**名前を付け**、「**[!UICONTROL プログラムタイプ]**」に「イベント」を選択します。

   ![](assets/import-a-list-of-people-5.png)

1. 「**[!UICONTROL チャネル]**」で「**[!UICONTROL トレードショー]**」を選択し、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>イベントプログラムは特定の日に発生します。[**イベント**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}&#x200B;の詳細をご覧ください。

## 手順 3：スプレッドシートを Marketo に読み込む {#step-import-your-spreadsheet-into-marketo}

1. **トレードショープログラム**&#x200B;で、「**[!UICONTROL 新規]**」をクリックし、「**[!UICONTROL 新規ローカルアセット]**」を選択します。

   ![](assets/import-a-list-of-people-7.png)

1. **[!UICONTROL リスト]**&#x200B;を選択します。

   ![](assets/import-a-list-of-people-8.png)

1. リストに「トレードショー参加者」という&#x200B;**名前を付け**、「**[!UICONTROL 作成]**」をクリックします。

   ![](assets/import-a-list-of-people-9.png)

1. **[!UICONTROL トレードショー参加者]**&#x200B;リストで、「**[!UICONTROL リストアクション]**」をクリックし、「**[!UICONTROL リストの読み込み]**」を選択します。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >独自の CSV ファイルを使用する場合は、エンコーディングが UTF-8、UTF-16、Shift-JIS、EUC-JP のいずれかであることを確認します。

   >[!NOTE]
   >
   >CSV ファイルのサイズの上限は 100MB です。

1. PC 上の **[!UICONTROL tradeshow-attendees.csv]** スプレッドシートファイルを&#x200B;**参照**&#x200B;し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >リストの読み込みモードで「**[!UICONTROL 新しい人物とアップデートをスキップ]**」を選択すると、既存の人物の記録やアクティビティのログには影響しません。マーケティングアクティビティで使用する既存の人物の、事前にフィルターされた迅速な静的リストを必要とする場合は、このモードを使用します。このモードを選択すると、以下の操作が行われます。
   >
   > * 新規人物の作成をスキップ
   > * 人物フィールドの更新をスキップ
   > * アクティビティログへの記録をスキップ

1. 「[!UICONTROL リスト列]」フィールドをそれぞれの Marketo フィールドにマッピングし、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >最適な自動マッピング結果を得るには、列ヘッダーは、常にフィールドと完全に一致する（大文字と小文字を区別）必要があります。カスタムフィールドを使用していて、ドロップダウンに表示されていない場合は、オプションになるように、戻って[作成](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}します。

   >[!NOTE]
   >
   >読み込まないフィールドがある場合は、Marketo フィールドドロップダウンメニューで&#x200B;**無視**&#x200B;を選択します。

1. **[!UICONTROL 新規顧客獲得プログラム]**&#x200B;に&#x200B;**マイトレードショープログラム**&#x200B;を選択し、「**[!UICONTROL 読み込み]**」をクリックします。

   ![](assets/import-a-list-of-people-13.png)

1. ユーザーが読み込むのを待ってから、読み込みの進行状況ポップアップを閉じます。

   ![](assets/import-a-list-of-people-14.png)

1. **トレードショープログラム**&#x200B;に戻り、「**[!UICONTROL メンバー]**」タブをクリックします。読み込んだすべての人物が表示されます。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>プログラムのメンバーシップをトラッキングすることで、プログラムの成功を分析できます。[**プログラム**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}&#x200B;の詳細をご覧ください。

## ミッション完了 {#mission-complete}

トレードショーの出席者は、Marketo プログラムのメンバーになりました。

<br>

[◄ミッション 4：メールの自動応答](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[ミッション 6：ドリップ、ドリップ、ナーチャリング►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
