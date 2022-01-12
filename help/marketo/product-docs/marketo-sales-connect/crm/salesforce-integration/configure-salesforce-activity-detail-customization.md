---
description: Salesforce アクティビティ詳細のカスタマイズの設定 — Marketoドキュメント — 製品ドキュメント
title: Salesforce アクティビティ詳細のカスタマイズの設定
hide: true
hidefromtoc: true
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: a95b889a36ae22aef6bc2ff5bc82f04751d389bd
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 3%

---

# Salesforce アクティビティ詳細のカスタマイズの設定 {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce とMarketo Sales Connect [は、接続されている必要があります](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* API を使用した電子メールアクティビティのログ [は有効にする必要があります](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)


アクティビティの詳細のカスタマイズを使用すると、管理者は、セールスコネクトのアクティビティ/リマインダータスクが Salesforce に同期されたときに、Salesforce タスク — 件名フィールドに記録する情報を設定できます。

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

この機能を使用して、次の利点をロック解除できます。

* 件名フィールドに表示される情報をカスタマイズすることで、Salesforce での販売に関するアクティビティの詳細を簡単にスキャンできます。
* 管理者は、件名フィールドに「Mkto_sales」などの一意の ID をタグ付けできるので、セールスコネクトのアクティビティを他のメールアクティビティ、通話アクティビティ、タスクと簡単に識別し、区別できます。
* カスタムアクティビティフィールドの必要性を減らします。 Salesforce では、カスタムアクティビティフィールドの数に制限が適用されるので、レポートで使用できるデータを制限できます。 アクティビティの動的フィールドを使用して主要データを件名行に追加することで、Salesforce インスタンスで作成する必要のあるカスタムアクティビティフィールドの数を減らすことができます。
* アクティビティとタスクの件名フィールドは、セールスコネクト管理者が定義した一貫したパターンに従います。

## サポートされるアクティビティの動的フィールド {#activity-dynamic-fields-supported}

アクティビティの動的フィールドは、データを入力するセールス活動に関する情報を参照します。 現在、Salesforce アクティビティ詳細カスタマイズと共に使用できます。

>[!NOTE]
>
>特定のアクティビティ/タスクの動的フィールドに値を入力する値がない場合、Salesforce タスク — 件名フィールドが更新されても、その動的フィールドのデータは入力されません。

<table>
 <tr>
  <th>フィールド</th>
  <th>説明</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>タスクタイプに [ 電子メール ]、[ 呼び出し ]、[InMail]、[ カスタム ] の値を設定します。</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>タスクの件名を入力します。</p>
      <p>E メールの場合は、E メールの件名行が入力されます。</p>
      <p>呼び出しの場合、inMail、または custom は、タスク名/件名フィールドに値を含むリマインダータスクが作成された場合に値を入力します。</p></td>
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
  <td>アクティビティがセールスキャンペーンから開始された場合は、このアクティビティが発生したセールスキャンペーン日内のステップ番号が入力されます。</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>アクティビティが呼び出しで、呼び出しの結果が選択されている場合は、呼び出しの結果値が設定されます。</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>「 」アクティビティが呼び出しで、呼び出しの理由が選択されている場合は、呼び出しの理由の値が設定されます。</td>
 </tr>
</table>

## Salesforce アクティビティ詳細のカスタマイズの設定 {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**管理者権限が必要です。**

アクティビティの詳細を設定する際は、Salesforce でタスク履歴を確認する際に、セールスに最も関連するデータを検討します。

1. 歯車アイコンをクリックし、「**設定**」を選択します。

PICC

1. クリック **Salesforce**.

PICC

1. クリック **同期設定**.

PICC

1. アクティビティ詳細のカスタマイズエディタで、任意のフリーテキストを追加します。Salesforce に同期されたすべてのタスクの件名フィールドは変更されません。

1. 追加するダイナミックフィールドを追加するには、ダイナミックフィールドボタンをクリックし、使用するダイナミックフィールドをリストから選択します。

1. 「**保存**」をクリックします。

>[!NOTE]
>
>Salesforce では 255 文字の制限が適用されます。 アクティビティの詳細がこれを超えると、情報を Salesforce 件名フィールドに保存できるように切り捨てられます。

>[!MORELIKETHIS]
>
>* [同期設定](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Salesforce とのリマインダータスク同期](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [CRM のセールスコネクトのカスタマイズ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)

