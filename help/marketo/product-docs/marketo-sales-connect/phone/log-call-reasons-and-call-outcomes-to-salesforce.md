---
description: Salesforce に通話理由と通話結果を記録 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce に通話理由と通話結果を記録
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 63%

---

# 通話理由と通話結果を [!DNL Salesforce] に記録する {#log-call-reasons-and-call-outcomes-to-salesforce}

レポートや表示の目的で、通話の結果と通話理由をログに記録し [!DNL Salesforce] い場合は、それぞれにカスタムアクティビティフィールドを作成できます。 各フィールドは、特定の API 名（[!DNL Salesforce] では「フィールド名」と呼ばれます）を使用する必要があります。

* 通話の結果フィールド名：mktosales_call_outcome
* 通話理由フィールド名：mktosales_call_reason

これらのフィールドを利用するには、まず、カスタムアクティビティフィールドとしてフィールドを作成する必要があります。ユーザに表示するには、タスクオブジェクトのページレイアウトに追加する必要があります。

## [!DNL Salesforce] Classic {#salesforce-classic}

### [!DNL Salesforce] Classic にカスタムアクティビティフィールドを作成  {#create-custom-activity-field-in-salesforce-classic}

1. [!DNL Salesforce] で、**[!UICONTROL 設定]** をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. クイック検索ボックスに「アクティビティ」と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. 「**[!UICONTROL アクティビティカスタムフィールド]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. データタイプ「[!UICONTROL &#x200B; テキスト &#x200B;]」を選択し、「次へ **[!UICONTROL をクリック]** ます。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. カスタムフィールドに、上で定義した名前を付けます。フィールドの長さの上限は 255 文字です。フィールドラベルは、セールスチームが表示できるフィールドで、チームのニーズに合わせてカスタマイズできます。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. 残りの設定はオプションです。設定が完了したら、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. このフィールドの目的のフィールドレベルのセキュリティ設定を選択し、「**[!UICONTROL 次へ]**」をクリックします（以下の画像は一例です）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >カスタムフィールドが、[!DNL Sales Connect] ユーザーが使用するプロファイルと、他の任意の表示したいプロファイルに対して表示されていることを確認します。

1. フィールドを追加するページレイアウトを選択し、「**[!UICONTROL 保存]**」をクリックします（オプションで、「**[!UICONTROL 保存して新規作成]**」をクリックし、「通話理由」フィールドに対してこのプロセスを繰り返すことができます）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### [!DNL Salesforce] Classic のタスクページレイアウトへのカスタムアクティビティフィールドの追加 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>上記の手順 9 で目的のページレイアウトを選択しなかった場合にのみ、これらの手順に従う必要があります。

1. [!DNL Salesforce] で、**[!UICONTROL 設定]** をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. クイック検索ボックスに「タスク」と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. 「**[!UICONTROL タスクページレイアウト]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. このフィールドを追加するタスクページレイアウトの横にある「**[!UICONTROL 編集]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. フィールドをタスクページレイアウトの目的のセクションにドラッグ＆ドロップします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## [!DNL Salesforce] Lightning {#salesforce-lightning}

### [!DNL Salesforce] Lightning でのカスタムアクティビティフィールドの作成 {#create-custom-activity-field-in-salesforce-lightning}

1. [!DNL Salesforce] で、右上の歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. 「**[!UICONTROL オブジェクトマネージャー]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. 「クイック検索」ボックスに「[!UICONTROL &#x200B; アクティビティ &#x200B;]」と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. 「**[!UICONTROL アクティビティ]**」ラベルをクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. 「**[!UICONTROL フィールドと関係]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. 「**[!UICONTROL 新規]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### [!DNL Salesforce] Lightning でタスクページレイアウトにカスタムアクティビティフィールドを追加する {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. [!DNL Salesforce] で、右上の歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. 「**[!UICONTROL オブジェクトマネージャー]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. 「クイック検索」ボックスに「[!UICONTROL Task]」と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. 「**[!UICONTROL タスク]**」ラベルをクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. 「**[!UICONTROL ページレイアウト]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. このフィールドを追加するタスクページレイアウトをクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. フィールドをタスクページレイアウトの目的のセクションにドラッグ＆ドロップします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[アクティビティ履歴への Sales Connect イベントフィールドのインストール](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
