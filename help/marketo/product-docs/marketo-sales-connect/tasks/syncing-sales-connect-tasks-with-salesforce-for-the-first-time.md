---
unique-page-id: 14352541
description: Sales Connect タスクと Salesforce の初回同期 - Marketo ドキュメント - 製品ドキュメント
title: Sales Connect タスクと Salesforce の初回同期
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '283'
ht-degree: 100%

---

# Sales Connect タスクと Salesforce の初回同期 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Sales Connect と Salesforce のタスク間の同期を初めて有効にすると、Salesforce のタスクがインポートされます。Sales Connect での現在のタスクは  Salesforce にプッシュされ&#x200B;**ません**。Sales Connect から Salesforce に同期されるタスクは、Sales Connect を SFDC と同期した&#x200B;*後に*&#x200B;作成されるタスクのみです。

Sales Connect と SFDC のタスクを同期すると、次の処理がおこなわれます。

- タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

- 過去 24 時間にアップデートまたは作成されたリマインダーは、SFDC から Sales Connect に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

- 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

- 同期が有効になっている限り、Sales Connect と SFDC の間でタスクが常に同期されます。

初回同期の後、Sales Connect で作成、編集、完了または削除したタスクは、Salesforce のタスクリストに同期されます。また、Salesforce でタスクが作成、編集、完了、削除されると、Sales Connect のタスクリストがアップデートされます。

この同期を有効にするには、Web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。
