---
unique-page-id: 14352541
description: Sales Connect タスクと Salesforce の初回同期 - Marketo ドキュメント - 製品ドキュメント
title: Sales Connect タスクと Salesforce の初回同期
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 48%

---

# [!DNL Sales Connect] タスクの [!DNL Salesforce] との初めての同期 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

最初に [!DNL Sales Connect] タスクと [!DNL Salesforce] タスクの同期を有効にすると、[!DNL Salesforce] タスクがインポートされます。 **に** して現在行ってい [!DNL Sales Connect] タスクは [!DNL Salesforce] 一切考慮しません」 煩雑さと重複を減らすために、[!DNL Sales Connect] から [!DNL Salesforce] に同期されるタスクは、作成されたタスク *後* のみ、[!DNL Sales Connect] をSFDCと同期します。

[!DNL Sales Connect] タスクとSFDC タスクを同期すると、次のようになります。

- タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

- 過去 24 時間以内に更新または作成されたリマインダーは、SFDCから [!DNL Sales Connect] に取り込まれます。 同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

- 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

- 同期が有効になっている限り、[!DNL Sales Connect] とSFDCの間でタスクを継続的に同期します。

最初の同期の後、[!DNL Sales Connect] で作成、編集、完了または削除したタスクは、[!DNL Salesforce] のタスクリストに同期されます。 [!DNL Salesforce] で作成、編集、完了または削除すると、[!DNL Sales Connect] のタスクリストが更新されます。

この同期を有効にするには、web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。
