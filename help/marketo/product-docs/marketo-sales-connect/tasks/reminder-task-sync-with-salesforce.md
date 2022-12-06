---
description: Salesforce とのリマインダータスク同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce とのリマインダータスク同期
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
source-git-commit: d2d6d4389f5a480afdfae6bfb62b9f48f0a2d88e
workflow-type: ht
source-wordcount: '564'
ht-degree: 100%

---

# Salesforce とのリマインダータスク同期 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>タスク同期を有効にする方法について詳しくは、[Sales Connect タスク／リマインダーの Salesforce タスクへの同期](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks)を参照してください。

タスクの同期設定が有効になると、ユーザは、Salesforce と双方向に同期されたリマインダータスクを確認できます。つまり、ユーザは Salesforce または Sales Connect からタスクを管理し、システムの整合性を維持していることを確信できます。

## リマインダータスクフィールドの同期 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下に、Sales Connect のリマインダータスクフィールドと、双方向タスク同期でサポートされる、対応する Salesforce フィールドの一覧を示します。

<table>
 <tr>
  <th>Sales Connect タスクフィールド</th>
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
  <td><p>タスクのステータスを表示します。Sales Connect タスクには、Salesforce タスクステータス選択リストの 2 つの値に対応する 2 つのステータスがあります。</p>
  <p>Sales Connect で開く = Salesforce で開始されていません。</p>
  <p>Sales Connect で完了 = Salesforce で完了</p>
  <p>Salesforce の他のステータス値は、Sales Connect に同期されません。</p></td>
 </tr>
 <tr>
  <td>優先度</td>
  <td>優先度</td>
  <td><p>Sales Connect の優先度は「標準」または「高」に設定でき、それらは Salesforce の「標準」と「高」の優先度値にマッピングされます。</p>
  <p>Salesforce の「低」優先度の値は、Sales Connect に同期されません。</p></td>
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

Sales Connect と Salesforce のタスク間の同期を初めて有効にすると、Salesforce のタスクがインポートされます。Sales Connect での現在のタスクは Salesforce にプッシュされ&#x200B;**ません**。Sales Connect から Salesforce に同期されるタスクは、Sales Connect を SFDC と同期した&#x200B;*後に*&#x200B;作成されるタスクのみです。

Sales Connect と SFDC のタスクを同期すると、次の処理が行われます。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間にアップデートまたは作成されたリマインダーは、SFDC から Sales Connect に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、Sales Connect と SFDC の間でタスクが常に同期されます。

初回同期の後、Sales Connect で作成、編集、完了または削除したタスクは、Salesforce のタスクリストに同期されます。また、Salesforce でタスクが作成、編集、完了、削除されると、Sales Connect のタスクリストがアップデートされます。

この同期を有効にするには、web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。

>[!NOTE]
>
>[アクティビティの詳細のカスタマイズ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md)設定で `{{activity_subject}}` 動的フィールドを使用している場合、タスクの件名フィールドは Sales Connect で更新でき、その更新は、対応する Salesforce タスクの件名フィールドに同期されます。逆に、Salesforce の件名フィールドを更新しても、Sales Connect のリマインダータスクの件名フィールドには&#x200B;_同期されません_。
