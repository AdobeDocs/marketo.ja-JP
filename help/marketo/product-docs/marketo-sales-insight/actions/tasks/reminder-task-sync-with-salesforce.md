---
description: Salesforce とのリマインダータスク同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce とのリマインダータスク同期
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 100%

---

# [!DNL Salesforce] とのリマインダータスク同期 {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>タスク同期を有効にする方法について詳しくは、[Sales Insight Actions タスク／リマインダーの Salesforce タスクへの同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks)を参照してください。

タスクの同期設定が有効になると、ユーザは、[!DNL Salesforce] と双方向に同期されたリマインダータスクを確認できます。つまり、ユーザは [!DNL Salesforce] または [!DNL Sales Insight Actions] からタスクを管理し、システムの整合性が維持されていることを確信できます。

## リマインダータスクフィールドの同期 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下に、[!DNL Sales Insight Actions] のリマインダータスクフィールドと、双方向タスク同期でサポートされる、対応する [!DNL Salesforce] フィールドの一覧を示します。

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] タスクフィールド</th>
  <th>[!DNL Salesforce] タスクフィールド</th>
  <th>[!DNL Salesforce] タスク</th>
 </tr>
 <tr>
  <td>[!UICONTROL タスク名]</td>
  <td>[!UICONTROL 件名フィールド]</td>
  <td>タスクのタイトルを示す短い概要フィールド。</td>
 </tr>
 <tr>
  <td>[!UICONTROL ステータス]</td>
  <td>[!UICONTROL タスクのステータス]</td>
  <td><p>タスクのステータスを表示します。[!DNL Sales Insight Actions] タスクには、[!DNL Salesforce] タスクステータス選択リストの 2 つの値に対応する 2 つのステータスがあります。</p>
  <p>[!DNL Sales Insight Actions] で開く = [!DNL Salesforce] で開始されていません。</p>
  <p>[!DNL Sales Insight Actions] で完了 = [!DNL Salesforce] で完了します。</p>
  <p>[!DNL Salesforce] の他のステータス値は、[!DNL Sales Insight Actions] に同期されません。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL 優先度]</td>
  <td>[!UICONTROL 優先度]</td>
  <td><p>[!DNL Sales Insight Actions] 優先度は「標準」または「高」に設定でき、それぞれ [!DNL Salesforce] の「標準」と「高」の優先度の値にマッピングされます。</p>
  <p>[!DNL Salesforce] の「低」優先度の値は、[!DNL Sales Insight Actions] に同期されません。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL 期日]</td>
  <td>[!UICONTROL 期日]</td>
  <td>タスクの期限。</td>
 </tr>
 <tr>
  <td>[!UICONTROL 詳細]</td>
  <td>[!UICONTROL コメント]</td>
  <td>リマインダータスクで完了する予定の内容に関する詳細情報を表示します。</td>
 </tr>
</table>

## [!DNL Sales Insight Actions] タスクの [!DNL Salesforce] との初めての同期 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

[!DNL Sales Insight Actions] と [!DNL Salesforce] のタスク間の同期を初めて有効にすると、[!DNL Salesforce] のタスクが読み込まれます。[!DNL Sales Insight Actions] の現在のタスクは [!DNL Salesforce] にプッシュ&#x200B;**されません**。[!DNL Sales Insight Actions] から [!DNL Salesforce] に同期されるタスクは、[!DNL Sales Insight Actions] を SFDC と同期した&#x200B;*後に*&#x200B;作成されるタスクのみです。

[!DNL Sales Insight Actions] と SFDC のタスクを同期すると、次の処理が行われます。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間に更新または作成されたリマインダーは、SFDC から [!DNL Sales Insight Actions] に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、[!DNL Sales Insight Actions] と SFDC の間でタスクが常に同期されます。

初回同期の後、[!DNL Sales Insight Actions] で作成、編集、完了または削除したタスクは、[!DNL Salesforce] のタスクリストに同期されます。また、[!DNL Salesforce] でタスクが作成、編集、完了、削除されると、[!DNL Sales Insight Actions] のタスクリストが更新されます。

この同期を有効にするには、web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。

>[!NOTE]
>
>[アクティビティの詳細のカスタマイズ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md)設定で `{{activity_subject}}` 動的フィールドを使用している場合、タスクの件名フィールドは [!DNL Sales Insight Actions] で更新でき、その更新は、対応する [!DNL Salesforce] タスクの件名フィールドに同期されます。逆に、[!DNL Salesforce] の件名フィールドを更新しても、[!DNL Sales Insight Actions] のリマインダータスクの件名フィールドには&#x200B;*同期されません*。
