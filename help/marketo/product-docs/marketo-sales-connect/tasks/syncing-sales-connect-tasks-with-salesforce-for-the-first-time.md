---
unique-page-id: 14352541
description: Sales Connect タスクと Salesforce の初回同期 - Marketo ドキュメント - 製品ドキュメント
title: Sales Connect タスクと Salesforce の初回同期
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 100%

---

# [!DNL Sales Connect] タスクと [!DNL Salesforce] の初回同期 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

[!DNL Sales Connect] と [!DNL Salesforce] のタスク間の同期を初めて有効にすると、[!DNL Salesforce] のタスクが読み込まれます。[!DNL Sales Connect] の現在のタスクは [!DNL Salesforce] にプッシュ&#x200B;**されません**。[!DNL Sales Connect] から [!DNL Salesforce] に同期されるタスクは、[!DNL Sales Connect] を SFDC と同期した&#x200B;*後に*&#x200B;作成されるタスクのみです。

[!DNL Sales Connect] と SFDC のタスクを同期すると、次の処理が行われます。

- タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

- 過去 24 時間に更新または作成されたリマインダーは、SFDC から [!DNL Sales Connect] に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

- 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

- 同期が有効になっている限り、[!DNL Sales Connect] と SFDC の間でタスクが常に同期されます。

初回同期の後、[!DNL Sales Connect] で作成、編集、完了または削除したタスクは、[!DNL Salesforce] のタスクリストに同期されます。また、[!DNL Salesforce] でタスクが作成、編集、完了、削除されると、[!DNL Sales Connect] のタスクリストが更新されます。

この同期を有効にするには、web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。
