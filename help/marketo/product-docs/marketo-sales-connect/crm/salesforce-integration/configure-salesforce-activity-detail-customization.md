---
description: Salesforce アクティビティ詳細のカスタマイズの設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce アクティビティ詳細のカスタマイズの設定
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 69%

---

# アクティビティ [!DNL Salesforce] 詳細のカスタマイズの設定 {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* [!DNL Salesforce] と [!DNL Marketo Sales Connect] [ 接続する必要があります ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* API を使用したメールアクティビティのログが[有効になっている](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)

アクティビティの詳細のカスタマイズにより、管理者は、[!DNL Sales Connect] しいアクティビティ/リマインダータスクがSalesforceに同期された際に、Salesforce タスク – 件名フィールドにログを記録する情報を設定できます。

>[!NOTE]
>
>* リマインダータスクの [!DNL Sales Connect] に件名フィールドに加えられた更新は、アクティビティの詳細のカスタマイズで [!DNL Salesforce] の動的フィールドを使用している場合、対応する `{{activity_subject}}` スタムタスクの件名フィールドに反映されます。
>* [!DNL Salesforce] の件名フィールドに情報を記録する場合、改行はサポートされていません。 セールスタスクの件名が更新されると、アクティビティ詳細のカスタマイズエディターで改行が削除されます。

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>InMail リマインダータスク</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>メールアクティビティ</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>通話アクティビティ</td>
 </tr>
</table>

この機能を使用して、以下のメリットをアンロックできます。

* 件名フィールドに表示される情報をカスタマイズすることで、Salesforce での販売に関するアクティビティの詳細を簡単にスキャンできます。
* 管理者は、件名フィールドに「Mkto_sales」などの一意の ID をタグ付けできるので、Sales Connect のアクティビティを簡単に識別し、他のメールアクティビティ、通話アクティビティ、タスクと区別できます。
* カスタムアクティビティフィールドの必要性を減らします。Salesforce では、カスタムアクティビティフィールドの数に制限が適用されるので、レポートで使用できるデータを制限できます。アクティビティの動的フィールドを使用して主要データを件名行に追加することで、Salesforce インスタンスで作成する必要のあるカスタムアクティビティフィールドの数を減らすことができます。
* アクティビティとタスクの件名フィールドは、Sales Connect 管理者が定義した一貫したパターンに従います。

>[!NOTE]
>
>メールの返信をアクティビティとして [!DNL Salesforce] に記録する場合、[!DNL Salesforce] のアクティビティの詳細のカスタマイズ設定は使用されません。 代わりに、「返信：メールの件名」として記録されます。

## サポートされるアクティビティの動的フィールド {#activity-dynamic-fields-supported}

アクティビティの動的フィールドでは、セールスアクティビティに関する情報を参照してデータが入力されます。現在は、アクティビティの詳細のカスタマイズ [!DNL Salesforce] 使用できます。

>[!NOTE]
>
>特定のアクティビティまたはタスクの動的フィールドに入力する値がない場合、[!DNL Salesforce] のタスク – 件名フィールドが更新されても、その動的フィールドのデータは入力されません。

<table>
 <tr>
  <th>フィールド</th>
  <th>説明</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>メール、呼び出し、InMail、カスタムのいずれかのタスクタイプが入力されます。</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>タスクの件名を入力します。</p>
      <p>メールの場合は、メールの件名行が入力されます。</p>
      <p>呼び出し、InMail、カスタムの場合、タスク名／件名フィールドに値を含むリマインダータスクが作成された場合に値が入力されます。</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>アクティビティがセールスキャンペーンから開始された場合は、セールスキャンペーンの名前が入力されます。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>アクティビティがセールスキャンペーンから開始された場合は、このアクティビティが発生したセールスキャンペーンの日番号が入力されます。</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>アクティビティがセールスキャンペーンから開始された場合は、このアクティビティが発生したセールスキャンペーン日内の手順番号が入力されます。</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>アクティビティが呼び出しで、呼び出しの結果が選択されている場合は、呼び出しの結果値が入力されます。</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>アクティビティが呼び出しで、呼び出しの理由が選択されている場合は、呼び出しの理由の値が入力されます。</td>
 </tr>
</table>

## Salesforce アクティビティ詳細のカスタマイズの設定 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**管理者権限が必要。**

アクティビティの詳細を設定する際は、[!DNL Salesforce] でタスク履歴を確認する際に、売上に最も関連のあるデータを検討します。

1. 歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. 「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. 「**[!UICONTROL 同期設定]**」をクリックします。

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. アクティビティの詳細のカスタマイズエディターで、任意のフリーテキストを追加します。追加したテキストは動的ではなく、[!DNL Salesforce] に同期されたすべてのタスクの件名フィールドに対して変更されません。

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >必須ではありませんが、追加したテキストを角括弧で囲むと、Salesforce の件名フィールドにデータを入力する際に、データ間の識別が容易になります。例：`[Sales Connect] - {{Activity_type}}`

1. 必要に応じて、「**[!UICONTROL 動的フィールドを追加]**」ボタンをクリックして、動的フィールドを追加します。

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. 目的の動的フィールドを選択します。

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>[!DNL Salesforce] では、255 文字制限が適用されます。 アクティビティの詳細がこの値を超えると、[!DNL Salesforce] の件名フィールドに情報が確実に保存されるように、内容が切り捨てられます。

>[!MORELIKETHIS]
>
>* [同期設定](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [ リマインダータスクの同期先  [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [[!DNL Sales Connect] CRM 向けカスタマイズ ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
