---
description: Salesforce とのリマインダータスク同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce とのリマインダータスク同期
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 34%

---

# リマインダータスクが [!DNL Salesforce] と同期されました {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>タスク同期を有効にする方法について詳しくは、[Sales Insight Actions タスク／リマインダーの Salesforce タスクへの同期](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks)を参照してください。

タスク同期設定が有効になると、リマインダータスクが [!DNL Salesforce] と双方向に同期されて表示されます。 つまり、ユーザーは [!DNL Salesforce] または [!DNL Sales Insight Actions] のどちらからでもタスクを管理でき、システムの整合性が確実に維持されていると感じることができます。

## リマインダータスクフィールドの同期 {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

以下は、[!DNL Sales Insight Actions] のリマインダータスクフィールドと、双方向のタスク同期でサポートされている対応するリマインダー [!DNL Salesforce] フィールドのリストです。

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] タスクフィールド</th>
  <th>[!DNL Salesforce] タスクフィールド</th>
  <th>[!DNL Salesforce] タスク</th>
 </tr>
 <tr>
  <td>[!UICONTROL タスク名 ]</td>
  <td>[!UICONTROL 件名フィールド ]</td>
  <td>タスクのタイトルを示す短い概要フィールドです。</td>
 </tr>
 <tr>
  <td>[!UICONTROL の状態 ]</td>
  <td>[!UICONTROL タスクの状態 ]</td>
  <td><p>タスクのステータスを表示します。[!DNL Sales Insight Actions] タスクには、[!DNL Salesforce] タスクの状態の選択リスト内の 2 つの値にマッピングされる 2 つの状態があります。</p>
  <p>[!DNL Sales Insight Actions] で開く= [!DNL Salesforce] で開始されていません。</p>
  <p>[!DNL Sales Insight Actions] に完了= [!DNL Salesforce] に完了します。</p>
  <p>[!DNL Salesforce] の他のステータス値は、[!DNL Sales Insight Actions] と同期されません。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL の優先度 ]</td>
  <td>[!UICONTROL の優先度 ]</td>
  <td><p>[!DNL Sales Insight Actions] 優先度は、Normal または High のいずれかであり、[!DNL Salesforce] の Normal および High の優先度の値にマップされます。</p>
  <p>[!DNL Salesforce] の優先度（低）の値は [!DNL Sales Insight Actions] と同期されません。</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL の期日 ]</td>
  <td>[!UICONTROL の期日 ]</td>
  <td>タスクの期限です。</td>
 </tr>
 <tr>
  <td>[!UICONTROL の詳細 ]</td>
  <td>[!UICONTROL コメント ]</td>
  <td>リマインダータスクで完了する予定の内容に関する詳細情報を表示します。</td>
 </tr>
</table>

## [!DNL Sales Insight Actions] タスクの [!DNL Salesforce] との初めての同期 {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

最初に [!DNL Sales Insight Actions] タスクと [!DNL Salesforce] タスクの同期を有効にすると、[!DNL Salesforce] タスクがインポートされます。 **に** して現在行ってい [!DNL Sales Insight Actions] タスクは [!DNL Salesforce] 一切考慮しません」 煩雑さと重複を減らすために、[!DNL Sales Insight Actions] から [!DNL Salesforce] に同期されるタスクは、作成されたタスク *後* のみ、[!DNL Sales Insight Actions] をSFDCと同期します。

[!DNL Sales Insight Actions] タスクとSFDC タスクを同期すると、次のようになります。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間以内に更新または作成されたリマインダーは、SFDCから [!DNL Sales Insight Actions] に取り込まれます。 同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、[!DNL Sales Insight Actions] とSFDCの間でタスクを継続的に同期します。

最初の同期の後、[!DNL Sales Insight Actions] で作成、編集、完了または削除したタスクは、[!DNL Salesforce] のタスクリストに同期されます。 [!DNL Salesforce] で作成、編集、完了または削除すると、[!DNL Sales Insight Actions] のタスクリストが更新されます。

この同期を有効にするには、web アプリケーションの[設定ページ](https://toutapp.com/login)で同期ボックスをオンにします。

>[!NOTE]
>
>[!DNL Sales Insight Actions] アクティビティの詳細のカスタマイズ [!DNL Salesforce] 設定で `{{activity_subject}}` の動的フィールドを使用している場合、タスクの件名フィールドを [ で更新でき、その更新が、対応する同期済みタスクの ](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) の件名フィールドで同期されます。 逆に、[!DNL Salesforce] の「件名」フィールドに行われた更新は、_リマインダータスクの「件名」フィールドに同期_ されません [!DNL Sales Insight Actions]。
