---
description: Salesforce とのリマインダータスク同期 — Marketoドキュメント — 製品ドキュメント
title: Salesforce とのリマインダータスク同期
hide: true
hidefromtoc: true
source-git-commit: 56db82ef98d774f8ac56c1401ef7ef275862d1dc
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 54%

---

# Salesforce とのリマインダータスク同期 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>タスク同期チェックアウトを有効にする方法を説明します [セールスコネクトタスク/Salesforce タスクのリマインダーを同期](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

タスクの同期設定が有効になると、ユーザーは、Salesforce と双方向に同期されたリマインダータスクを確認できます。 つまり、ユーザーは Salesforce またはセールスコネクトからタスクを管理し、システムの整合性を維持できると確信します。

## リマインダータスクフィールドの同期 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下に、セールスコネクトのリマインダータスクフィールドと、双方向タスク同期でサポートされる対応する Salesforce フィールドの一覧を示します。

<table>
 <tr>
  <th>セールスコネクトタスクフィールド</th>
  <th>Salesforce タスクフィールド</th>
  <th>Salesforce タスク</th>
 </tr>
 <tr>
  <td>タスク名</td>
  <td>件名フィールド</td>
  <td>タスクのタイトルを示す短い概要フィールドです。</td>
 </tr>
 <tr>
  <td>ステータス</td>
  <td>タスクのステータス</td>
  <td><p>タスクのステータスを表示します。 セールスコネクトタスクには、Salesforce タスクステータス選択リストの 2 つの値に対応する 2 つのステータスがあります。</p>
  <p>セールスコネクトで開く= Salesforce で開始されていません。</p>
  <p>セールスコネクトで完了= Salesforce で完了</p>
  <p>Salesforce の他のステータス値は、セールスコネクトに同期されません。</p></td>
 </tr>
 <tr>
  <td>優先度</td>
  <td>優先度</td>
  <td><p>セールスコネクトの優先度は、Salesforce の「標準」と「高」の優先度値にマッピングされる「標準」または「高」に設定できます。</p>
  <p>Salesforce の低優先度の値は、セールスコネクトに同期されません。</p></td>
 </tr>
 <tr>
  <td>期日</td>
  <td>期日</td>
  <td>タスクの期限です。</td>
 </tr>
 <tr>
  <td>詳細</td>
  <td>コメント</td>
  <td>リマインダータスクで完了する予定の内容に関する詳細情報を表示します。</td>
 </tr>
</table>

## Sales Connect タスクと Salesforce の初回同期 {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Sales Connect と Salesforce のタスク間の同期を初めて有効にすると、Salesforce のタスクがインポートされます。Sales Connect での現在のタスクは  Salesforce にプッシュされ&#x200B;**ません**。Sales Connect から Salesforce に同期されるタスクは、Sales Connect を SFDC と同期した&#x200B;*後に*&#x200B;作成されるタスクのみです。

Sales Connect と SFDC のタスクを同期すると、次の処理がおこなわれます。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間にアップデートまたは作成されたリマインダーは、SFDC から Sales Connect に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、Sales Connect と SFDC の間でタスクが常に同期されます。

初回同期の後、Sales Connect で作成、編集、完了または削除したタスクは、Salesforce のタスクリストに同期されます。また、Salesforce でタスクが作成、編集、完了、削除されると、Sales Connect のタスクリストがアップデートされます。

この同期を有効にするには、Web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。
