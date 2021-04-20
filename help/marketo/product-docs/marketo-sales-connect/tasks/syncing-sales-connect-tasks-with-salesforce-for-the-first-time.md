---
unique-page-id: 14352541
description: Sales ConnectタスクとSalesforceとの初回同期 —Marketoドキュメント — 製品ドキュメント
title: Sales ConnectタスクとSalesforceとの初回同期
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Sales ConnectタスクとSalesforceとの初回同期{#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Sales ConnectとSalesforceのタスク間の同期を最初にオンにしたとき、Salesforceのタスクをインポートします。 Sales ConnectからSalesforceへの現在のタスクは&#x200B;**押し上げません**。 Sales ConnectからSalesforceに同期されるタスクは、Sales ConnectをSFDCと同期した後に&#x200B;*作成されたタスクのみで、混乱や重複を減らすためです。*

Sales ConnectとSFDCのタスクを同期すると、次のようになります。

- 同期するタスクの保存をクリックすると、同期が開始されます。 最初は、この処理には時間がかかります。

- 過去24時間に更新または作成されたリマインダーは、SFDCからSales Connectに取り込まれます。 同期は期限に基づいており、これらのすべてのタスクはバックエンドで同期されますが、コマンドセンターでは、期限が今日と明日のみのタスクが表示されます。

- 同期が有効になっていて、SFDC内のタスクを削除した場合、過去15日間に削除されたすべての要素はコマンドセンターから削除されます。

- 同期が有効である限り、Sales ConnectとSFDCの間でタスクを常に同期します。

最初の同期後、Sales Connectで作成、編集、完了または削除したタスクは、Salesforceのタスクリストに同期されます。 また、Salesforceで作成、編集、完了、または削除されたものはすべて、Sales Connectでタスクリストを更新します。

この同期を有効にするには、Webアプリケーションの[設定ページ](https://toutapp.com/login)の同期ボックスをオンにします。
