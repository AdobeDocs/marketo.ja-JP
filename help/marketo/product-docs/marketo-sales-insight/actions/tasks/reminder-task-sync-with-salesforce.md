---
description: Salesforce とのリマインダータスク同期 — Marketoドキュメント — 製品ドキュメント
title: Salesforce とのリマインダータスク同期
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 21%

---

# Salesforce とのリマインダータスク同期 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>タスク同期チェックアウトを有効にする方法を説明します [Sales Insight アクションタスク/Salesforce タスクへのリマインダーを同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

タスクの同期設定が有効になると、ユーザーは、Salesforce と双方向に同期されたリマインダータスクを確認できます。 つまり、ユーザーは Salesforce または Sales Insight のアクションからタスクを管理し、システムの整合性を維持できると確信します。

## リマインダータスクフィールドの同期 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下は、Sales Insight アクションのリマインダータスクフィールドと、双方向タスク同期でサポートされる対応する Salesforce フィールドの一覧です。

<table>
 <tr>
  <th>Sales Insight アクションタスクフィールド</th>
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
  <td><p>タスクのステータスを表示します。 Sales Insight アクションタスクには、Salesforce タスクステータス選択リストの 2 つの値に対応する 2 つのステータスがあります。</p>
  <p>Sales Insight のアクションで開く= Salesforce で開始されていません。</p>
  <p>Sales Insight でのアクションの完了= Salesforce で完了。</p>
  <p>Salesforce の他のステータス値は、Sales Insight アクションと同期されません。</p></td>
 </tr>
 <tr>
  <td>優先度</td>
  <td>優先度</td>
  <td><p>Sales Insight アクションの優先度は、Salesforce の「標準」と「高」のどちらかの値にマッピングされる「標準」または「高」に設定できます。</p>
  <p>Salesforce の低優先度の値は、Sales Insight アクションと同期されません。</p></td>
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

## Sales Insight のアクションタスクを Salesforce と初めて同期 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Sales Insight アクションと Salesforce タスクの同期を初めて有効にすると、Salesforce タスクがインポートされます。 我々は **not** Sales Insight アクションの現在のタスクを Salesforce にプッシュします。 混乱や重複を減らすために、Sales Insight アクションから Salesforce に同期されるタスクは、作成されたタスクのみです *後* Sales Insight のアクションを SFDC と同期します。

Sales Insight のアクションと SFDC タスクを同期すると、次の処理が行われます。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間に更新または作成されたリマインダーは、SFDC から Sales Insight アクションに取り込まれます。 同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、Sales Insight Actions と SFDC の間でタスクを常に同期します。

初回同期後、Sales Insight アクションで作成、編集、完了、削除したタスクは、Salesforce のタスクリストに同期されます。 また、Salesforce で作成、編集、完了、または削除されたすべての項目は、Sales Insight アクションのタスクリストを更新します。

この同期を有効にするには、Web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。

>[!NOTE]
>
>タスクの件名フィールドを Sales Insight アクションで更新すると、対応する同期済みタスクの Salesforce 件名フィールド ( `{{activity_subject}}` 動的フィールドを [アクティビティの詳細のカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) 設定。 反対に、Salesforce の件名フィールドに対して行われた更新は、 _not_ [Sales Insight Actions リマインダータスクの件名 ] フィールドに同期します。
