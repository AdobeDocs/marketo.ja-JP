---
unique-page-id: 14352541
description: Sales ConnectタスクとSalesforceとの初回同期 — Marketto Docs — 製品ドキュメント
title: Sales ConnectタスクとSalesforceとの初回同期
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Sales ConnectタスクとSalesforceとの初回同期 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Sales ConnectとSalesforceのタスク間の同期を最初にオンにしたとき、Salesforceのタスクをインポートします。 Sales ConnectからSalesforceへの現在のタスク **は引き継がれません** 。 混乱や重複を減らすために、Sales ConnectからSalesforceに同期されるタスクは、Sales ConnectをSFDCと同期した *後に作成されるタスクのみです* 。

Sales ConnectとSFDCのタスクを同期すると、次のようになります。

- 同期するタスクの保存をクリックすると、同期が開始されます。 最初は、この処理には時間がかかります。

- で更新または作成されたリマインダーは、SFDCからSales Connectに取り込ま `last 24 hours` れます。 同期は基になり、これらのすべてのタスクはバックエンドで同期されますが、コマンドセンターでは、今日および明日の期限のタスクのみが表示されます。 `due date`

- 同期が有効になっていて、SFDC内のタスクを削除した場合、過去15日間に削除されたすべての要素はコマンドセンターから削除されます。

- 同期が有効である限り、Sales ConnectとSFDCの間でタスクを常に同期します。

最初の同期後、Sales Connectで作成、編集、完了または削除したタスクは、Salesforceのタスクリストに同期されます。 また、Salesforceで作成、編集、完了、または削除されたものはすべて、Sales Connectでタスクリストを更新します。

この同期を有効にするには、Webアプリケーションの [設定ページ](http://toutapp.com/next#settings/crm/salesforce/configure) の同期ボックスをオンにします。

