---
description: セールスアクティビティの Salesforce への同期 - Marketo ドキュメント - 製品ドキュメント
title: セールスアクティビティの Salesforce への同期
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: ht
source-wordcount: '759'
ht-degree: 100%

---

# セールスアクティビティの Salesforce への同期 {#sync-sales-activities-to-salesforce}

メールおよび電話アクティビティを Salesforce に記録するための Actions Salesforce 同期設定を設定できます。これにより、チームは、CRM での作業を視認しやすくなり、マネージャーは、これらのアクティビティを使用してチームのパフォーマンスをトラッキングするためのカスタム Salesforce レポートを作成できます。

## メールアクティビティのログを API 経由で Salesforce に記録 {#logging-email-activity-to-salesforce-via-api}

この機能を使用するには、Salesforce の Enterprise／Unlimited エディション、または web サービス API を通じて統合を購入済みの場合は Professional エディションを使用する必要があります。

>[!PREREQUISITES]
>
>Salesforce と Sales Insight Actions を接続する必要があります。

1. Sales Insight Actions で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/sync-sales-activities-to-salesforce-1.png)

1. 「管理者設定」（または管理者でない場合は「マイアカウント」）で、**Salesforce**.をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-2.png)

1. 「**同期設定**」タブをクリックします。

   ![](assets/sync-sales-activities-to-salesforce-3.png)

1. 「メールアクティビティのログを Salesforce に記録」の横の矢印をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-4.png)

1. 「**Salesforce API**」タブをクリックします。このカードでは、Salesforce に情報を記録する際の環境設定を設定できます。終了したら「**保存**」をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-5.png)

## メールアクティビティのログを Salesforce にメール送信（BCC）して Salesforce に記録 {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

「Salesforce にメールを送信（BCC）」を有効にすると、セールスメールの BCC が送信され、メールは商談、リード、連絡先に関するアクティビティとして記録されます。

>[!PREREQUISITES]
>
>Salesforce と Sales Insight Actions を接続する必要があります。

**メール（BCC）を使用して Salesforce にメールを記録するには**

1. Marketo Sales で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/sync-sales-activities-to-salesforce-6.png)

1. 「管理者設定」（または管理者でない場合は「マイアカウント」）で、**Salesforce**.をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-7.png)

1. 「**同期設定**」タブをクリックします。

   ![](assets/sync-sales-activities-to-salesforce-8.png)

1. 「**Salesforce にメールを送信（BCC）**」タブをクリックし、「**有効化**」をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-9.png)

何らかの理由で Salesforce へのメールアドレスが取り込まれない場合は、以下の手順に従って、Salesforce アカウントで BCC 機能を有効にします。

1. Salesforce インスタンスにログインします。
1. 右上隅にあるユーザー名を探し、ドロップダウンバーを選択します。
1. 「**マイ設定**」を選択します。
1. 「**メール**」を選択します。
1. 「**メールを Salesforce に送信**」を選択します。
1. このページに、「Salesforce アドレス宛てにメールを送信」というラベルの付いたフィールドが表示されます。横に何も入力されていない場合は、「アクセス可能なメールアドレス」までスクロールします。
1. BCC を送信するメールアドレスを入力します。
1. 「**変更を保存**」をクリックします。

**マイ設定で Salesforce へのメール送信が見つからない**

「設定」に「Salesforce へのメール送信」が表示されない場合は、管理者が有効にしていない可能性があります。これは、チームが Salesforce を初めて使用した場合や、チームが Salesforce が提供する BCC アドレスを使用したことがない場合に発生する可能性があります。

>[!NOTE]
>
>これを設定するには、管理者権限が必要です。

1. 「**設定**」をクリックします。
1. 「**メール管理**」をクリックします。
1. 「**Salesforce にメール送信**」をクリックします。
1. 「**編集**」をクリックします。
1. 「アクティブ」の横のボックスをオンにします。
1. 「**保存**」をクリックします。

## Sales Insight Actions タスク／リマインダーを同期 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. Sales Insight Actions で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/sync-sales-activities-to-salesforce-10.png)

1. 「管理者設定」（または管理者でない場合は「マイアカウント」）で、**Salesforce**.をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-11.png)

1. 「**同期設定**」タブをクリックします。

   ![](assets/sync-sales-activities-to-salesforce-12.png)

1. 「Marketo Sales タスク／リマインダーを Salesforce タスクに同期」の横の矢印をクリックします。

   ![](assets/sync-sales-activities-to-salesforce-13.png)

1. 目的のオプションを選択します（「Salesforce タスクに同期しない」がデフォルトで選択されています）。

   ![](assets/sync-sales-activities-to-salesforce-14.png)

## Sales Insight Actions タスクと Salesforce の初回同期 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Sales Insight Actions と Salesforce のタスク間の同期を初めて有効にすると、Salesforce のタスクがインポートされます。Sales Insight Actions の現在のタスクは Salesforce にプッシュされません。Sales Insight Actions から Salesforce に同期されるタスクは、Sales Insight Actions を SFDC と同期した後に作成されるタスクのみです。

Sales Insight Actions と SFDC のタスクを同期すると、以下の処理が行われます。

* タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

* 過去 24 時間にアップデートまたは作成されたリマインダーは、SFDC から Sales Insight Actions に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

* 同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

* 同期が有効になっている限り、Sales Insight Actions と SFDC の間でタスクが常に同期されます。

* 初回同期の後、Sales Insight Actions で作成、編集、完了または削除したタスクは、Salesforce のタスクリストに同期されます。また、Salesforce でタスクが作成、編集、完了、削除されると、Sales Insight Actions のタスクリストがアップデートされます。

* この同期を有効にするには、web アプリケーションの設定ページで同期ボックスをオンにします。
