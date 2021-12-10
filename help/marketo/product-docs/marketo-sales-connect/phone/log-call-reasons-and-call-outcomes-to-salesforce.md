---
description: Salesforce に対するログ呼び出し理由と呼び出し結果 — Marketoドキュメント — 製品ドキュメント
title: Salesforce に通話理由と通話結果を記録
hide: true
hidefromtoc: true
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
source-git-commit: 357da216508db6196042d07000cbc1b04fa41071
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 4%

---

# Salesforce に通話理由と通話結果を記録 {#log-call-reasons-and-call-outcomes-to-salesforce}

レポートや表示の目的で、通話の結果や通話理由を Salesforce に記録したい場合は、それぞれにカスタムアクティビティフィールドを作成できます。 各フィールドは、特定の API 名（Salesforce では「フィールド名」と呼ばれます）を使用する必要があります。

* 通話の結果フィールド名：mktosales_call_outcome
* 通話理由フィールド名：mktosales_call_reason

これらのフィールドを利用するには、まず、カスタムアクティビティフィールドとしてフィールドを作成する必要があります。 ユーザーに表示するには、タスクオブジェクトのページレイアウトに追加する必要があります。

## Salesforce Classic {#salesforce-classic}

### Salesforce Classic でカスタムアクティビティフィールドを作成  {#create-custom-activity-field-in-salesforce-classic}

1. Salesforce で、 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. クイック検索ボックスに&quot;Activitys&quot;と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. クリック **アクティビティカスタムフィールド**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. 「**新規**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. データタイプ「テキスト」を選択し、 **次へ**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. カスタムフィールドに、上で定義した名前を付けます。 フィールドの長さの上限は 255 文字です。 フィールドラベルは、セールスチームが表示できるフィールドで、チームのニーズに合わせてカスタマイズできます。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. 残りの設定はオプションです。 設定が完了したら、「 **次へ**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. このフィールドの目的のフィールドレベルのセキュリティ設定を選択し、 **次へ** （以下の画像は一例です）。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >セールスコネクトユーザーが使用するプロファイルと、他に表示したいプロファイルにカスタムフィールドが表示されていることを確認します。

1. フィールドを追加するページレイアウトを選択し、 **保存** ( オプションで、 **保存して新規作成** 「Call Reason」フィールドのプロセスを繰り返します )。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Salesforce Classic のタスクページレイアウトにカスタムアクティビティフィールドを追加 {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>上記の手順 9 で目的のページレイアウトを選択しなかった場合にのみ、これらの手順に従う必要があります。

1. Salesforce で、 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. [ クイック検索 ] ボックスに&quot;タスク&quot;と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. クリック **タスクページレイアウト**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. クリック **編集** このフィールドを追加するタスクページレイアウトの横にあります。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. フィールドをタスクページレイアウトの目的のセクションにドラッグ&amp;ドロップします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. 「**保存**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Salesforce Lightning でカスタムアクティビティフィールドを作成 {#create-custom-activity-field-in-salesforce-lightning}

1. Salesforce で、右上の歯車アイコンをクリックし、「 」を選択します。 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. クリック **オブジェクトマネージャ**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. クイック検索ボックスに&quot;Activity&quot;と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. 次をクリック： **アクティビティ** ラベル

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. クリック **フィールドと関係**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. 「**新規**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

## Salesforce Lightning のタスクページレイアウトにカスタムアクティビティフィールドを追加 {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. Salesforce で、右上の歯車アイコンをクリックし、「 」を選択します。 **設定**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. クリック **オブジェクトマネージャ**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. [ クイック検索 ] ボックスに&quot;タスク&quot;と入力します。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. 次をクリック： **タスク** ラベル

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. 「**ページレイアウト**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. このフィールドを追加するタスクページレイアウトを pn ボタンでクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. フィールドをタスクページレイアウトの目的のセクションにドラッグ&amp;ドロップします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. 「**保存**」をクリックします。

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[アクティビティ履歴への Sales Connect イベントフィールドのインストール](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
