---
description: Salesforce とのリマインダータスク同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce とのリマインダータスク同期
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: ht
source-wordcount: '586'
ht-degree: 100%

---

# Salesforce とのリマインダータスク同期 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>タスク同期を有効にする方法について詳しくは、[Sales Insight Actions タスク／リマインダーの Salesforce タスクへの同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks)を参照してください。

タスクの同期設定が有効になると、ユーザは、Salesforce と双方向に同期されたリマインダータスクを確認できます。つまり、ユーザは Salesforce または Sales Insight Actions からタスクを管理し、システムの整合性を維持していることを確信できます。

## リマインダータスクフィールドの同期 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下に、Sales Insight Actions のリマインダータスクフィールドと、双方向タスク同期でサポートされる、対応する Salesforce フィールドの一覧を示します。

<table>
 <tr>
  <th>Sales Insight Actions タスクフィールド</th>
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
  <td><p>タスクのステータスを表示します。Sales Insight Actions タスクには、Salesforce タスクステータス選択リストの 2 つの値に対応する 2 つのステータスがあります。</p>
  <p>Sales Insight Actions で開く = Salesforce で開始されていません。</p>
  <p>Sales Insight Actions で完了 = Salesforce で完了</p>
  <p>Salesforce の他のステータス値は、Sales Insight Actions に同期されません。</p></td>
 </tr>
 <tr>
  <td>優先度</td>
  <td>優先度</td>
  <td><p>Sales Insight Actions の優先度は「標準」または「高」に設定でき、それらは Salesforce の「標準」と「高」の優先度値にマッピングされます。</p>
  <p>Salesforce の「低」優先度の値は、Sales Insight Actions に同期されません。</p></td>
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

## Sales Insight Actions タスクと Salesforce の初回同期 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Sales Insight Actions と Salesforce のタスク間の同期を初めて有効にすると、Salesforce のタスクがインポートされます。Sales Insight Actions の現在のタスクは Salesforce にプッシュ&#x200B;**されません**。Sales Insight Actions から Salesforce に同期されるタスクは、Sales Insight Actions を SFDC と同期した&#x200B;*後*&#x200B;に作成されるタスクのみです。

Sales Insight Actions と SFDC のタスクを同期すると、次の処理が行われます。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間にアップデートまたは作成されたリマインダーは、SFDC から Sales Insight Actions に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、Sales Insight Actions と SFDC の間でタスクが常に同期されます。

初回同期の後、Sales Insight Actions で作成、編集、完了または削除したタスクは、Salesforce のタスクリストに同期されます。また、Salesforce でタスクが作成、編集、完了、削除されると、Sales Insight Actions のタスクリストがアップデートされます。

この同期を有効にするには、web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。

>[!NOTE]
>
>[アクティビティの詳細のカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md)設定で `{{activity_subject}}` 動的フィールドを使用している場合、タスクの件名フィールドは Sales Insight Actions で更新でき、その更新は、対応する Salesforce タスクの件名フィールドに同期されます。逆に、Salesforce の件名フィールドを更新しても、Sales Insight Actions のリマインダータスクの件名フィールドには&#x200B;_同期されません_。
