---
unique-page-id: 2359418
description: 人物のリストのインポート - Marketo ドキュメント - 製品ドキュメント
title: 人物のリストのインポート
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: a61f9c2bbfd7c6b4c34fd1731698dc90ad1bd6cf
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 89%

---

# 人物のリストのインポート {#import-a-list-of-people}

## ミッション：トレードショーの出席者のスプレッドシートリストをデータベースに読み込む {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[セットアップと人物の追加](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}

このチュートリアルでは、スプレッドシートファイルから Marketo に人物を読み込む方法を学びます。

## 手順 1：スプレッドシートをダウンロード／編集する {#step-download-and-edit-a-spreadsheet}

1. まず、プラクティスのスプレッドシートファイル ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target=&quot;_blank&quot;}) をコンピューターに送信します。

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >日付を読み込む場合は、次の形式を使用します。**9/21/20**（月/日/年）。

   >[!NOTE]
   >
   >読み込まれる日時フィールドは、すべて米中央時間として扱われます。日時フィールドのタイムゾーンが異なる場合、Excel の数式を使用して、中央時刻（米国／シカゴ）に変換できます。

1. 自分の姓、名、実際のメールアドレス（次のミッションで送信するメールを受け取れるように）、役職を追加します。ファイルをコンピューターに保存します。

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >Marketo は、絵文字を含むメールアドレスを&#x200B;**サポートしていません**。

## 手順 2：プログラムを作成する {#step-create-a-program}

1. **マーケティングアクティビティ**&#x200B;領域に移動します。

   ![](assets/import-a-list-of-people-3.png)

1. **学習**&#x200B;フォルダーを選択し、「**新規**」で「**新規プログラム**」をクリックします。

   ![](assets/import-a-list-of-people-4.png)

1. プログラムに「トレードショープログラム」と&#x200B;**名前を付け**、「**プログラムタイプ**」に「イベント」を選択します。

   ![](assets/import-a-list-of-people-5.png)

1. 「**チャネル**」で「**トレードショー**」を選択し、「**作成**」をクリックします。

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>イベントプログラムは特定の日に発生します。詳細情報： [**イベント**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target=&quot;_blank&quot;}。

## 手順 3：スプレッドシートを Marketo に読み込む {#step-import-your-spreadsheet-into-marketo}

1. **トレードショープログラム**&#x200B;で、「**新規**」をクリックし、「**新規ローカルアセット**」を選択します。

   ![](assets/import-a-list-of-people-7.png)

1. 選択 **リスト**.

   ![](assets/import-a-list-of-people-8.png)

1. リストに「トレードショー参加者」という&#x200B;**名前を付け**、「**作成**」をクリックします。

   ![](assets/import-a-list-of-people-9.png)

1. **トレードショー参加者**&#x200B;リストで、「**リストアクション**」をクリックし、「**リストの読み込み**」を選択します。

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >独自の CSV ファイルを使用する場合は、エンコーディングが UTF-8、UTF-16、Shift-JIS、EUC-JP のいずれかであることを確認します。

   >[!NOTE]
   >
   >CSV ファイルのサイズの上限は 100MB です。

1. PC 上の **tradeshow-attendees.csv** スプレッドシートファイルを&#x200B;**参照**&#x200B;し、「**次へ**」をクリックします。

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >リストの読み込みモードで「**新しい人物とアップデートをスキップ**」を選択すると、既存の人物の記録やアクティビティのログには影響しません。マーケティングアクティビティで使用する既存の人物の、事前にフィルターされた迅速な静的リストを必要とする場合は、このモードを使用します。このモードを選択すると、次の操作がおこなわれます。
   >
   > * 新規人物の作成をスキップ
   > * 人物フィールドの更新をスキップ
   > * アクティビティログへの記録をスキップ


1. 「リスト列」フィールドをそれぞれの Marketo フィールドにマッピングし、「**次へ**」をクリックします。

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >最適な自動マッピング結果を得るには、列ヘッダーは、常にフィールドと完全に一致する（大文字と小文字を区別）必要があります。カスタムフィールドを使用していて、ドロップダウンに表示されない場合は、戻って [作成する](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;} を使用して、これらをオプションにすることができます。

   >[!NOTE]
   >
   >読み込まないフィールドがある場合は、Marketo フィールドドロップダウンメニューで「**無視**」を選択します。

1. **獲得プログラム**&#x200B;に&#x200B;**マイトレードショープログラム**&#x200B;を選択し、「**読み込み**」をクリックします。

   ![](assets/import-a-list-of-people-13.png)

1. ユーザーが読み込むのを待ってから、読み込みの進行状況ポップアップを閉じます。

   ![](assets/import-a-list-of-people-14.png)

1. **トレードショープログラム**&#x200B;に戻り、「**メンバー**」タブをクリックします。読み込んだすべての人物が表示されます。

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>プログラムのメンバーシップを追跡することで、プログラムの成功を分析できます。詳細情報： [**プログラム**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;}。

## ミッション完了 {#mission-complete}

トレードショーの出席者は、Marketo プログラムのメンバーになりました。

<br> 

[◄ ミッション 4：メールの自動応答](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[ミッション 6：ドリップ、ドリップ、ナーチャリング ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
