---
description: Salesforce 同期設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce 同期設定
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 100%

---

# [!DNL Salesforce] 同期設定 {#salesforce-sync-settings}

## メールアクティビティのログを API 経由で [!DNL Salesforce] に記録 {#logging-email-activity-to-salesforce-via-api}

この機能を使用するには、[!DNL Salesforce] の Enterprise／Unlimited エディション、または Professional エディション（Web Services API を通じて統合を購入済みの場合）を使用する必要があります。

>[!PREREQUISITES]
>
>[!DNL Salesforce] および [!DNL Sales Insight Actions] を接続する必要があります。

1. [!DNL Sales Insight Actions] で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/salesforce-sync-settings-1.png)

1. 「[!UICONTROL 管理者設定]」（または管理者でない場合は「[!UICONTROL マイアカウント]」）で、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/salesforce-sync-settings-2.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/salesforce-sync-settings-3.png)

1. [!DNL Salesforce] への「[!UICONTROL メールアクティビティのログを記録]」の横の矢印をクリックします。

   ![](assets/salesforce-sync-settings-4.png)

1. 「**[!UICONTROL Salesforce API]**」タブをクリックします。このカードでは、[!DNL Salesforce] に情報を記録する際の環境設定を設定できます。終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/salesforce-sync-settings-5.png)

## メールアクティビティのログを [!DNL Salesforce] にメール送信（BCC）して [!DNL Salesforce] に記録 {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

「[!UICONTROL Salesforce にメールを送信（BCC）]」を有効にすると、セールスメールの BCC が送信され、メールは商談、リード、取引先責任者に関するアクティビティとして記録されます。

>[!PREREQUISITES]
>
>[!DNL Salesforce] および [!DNL Sales Insight Actions] を接続する必要があります。

**メール（BCC）を使用して [!DNL Salesforce] にメールを記録するには**

1. Marketo Sales で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/salesforce-sync-settings-6.png)

1. 「[!UICONTROL 管理者設定]」（または管理者でない場合は「[!UICONTROL マイアカウント]」）で、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/salesforce-sync-settings-7.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/salesforce-sync-settings-8.png)

1. 「**[!UICONTROL Salesforce にメールを送信（BCC）]**」タブをクリックし、「**[!UICONTROL 有効化]**」をクリックします。

   ![](assets/salesforce-sync-settings-9.png)

何らかの理由で [!DNL Salesforce] へのメールアドレスが取り込まれない場合は、以下の手順に従って、[!DNL Salesforce] アカウントで BCC 機能を有効にします。

1. [!DNL Salesforce] インスタンスにログインします。
1. 右上隅にあるユーザー名を探し、ドロップダウンバーを選択します。
1. 「**[!UICONTROL マイ設定]**」を選択します。
1. 「**[!UICONTROL メール]**」を選択します。
1. 「**[!UICONTROL メールを Salesforce に送信]**」を選択します。
1. このページに、「[!UICONTROL Salesforce アドレス宛てにメールを送信]」というラベルの付いたフィールドが表示されます。横に何も入力されていない場合は、「[!UICONTROL アクセス可能なメールアドレス]」までスクロールします。
1. BCC を送信するメールアドレスを入力します。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

**マイ設定で [!DNL Salesforce] へのメール送信が見つからない**

「設定」に「[!DNL Salesforce] へのメール送信」が表示されない場合は、管理者が有効にしていない可能性があります。これは、チームが [!DNL Salesforce] を初めて使用した場合や、チームが [!DNL Salesforce] が提供する BCC アドレスを使用したことがない場合に発生する可能性があります。

>[!NOTE]
>
>これを設定するには、管理者権限が必要です。

1. 「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL メール管理]**」をクリックします。
1. 「**[!UICONTROL Salesforce にメール送信]**」をクリックします。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. 「アクティブ」の横のボックスをオンにします。
1. 「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Sales Insight Actions] タスク／[!DNL Salesforce] タスクのリマインダーを同期 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. [!DNL Sales Insight Actions] で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/salesforce-sync-settings-10.png)

1. 「[!UICONTROL 管理者設定]」（または管理者でない場合は「[!UICONTROL マイアカウント]」）で、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/salesforce-sync-settings-11.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/salesforce-sync-settings-12.png)

1. 「Marketo Sales タスク／[!DNL Salesforce] タスクのリマインダーを同期」の横の矢印をクリックします。

   ![](assets/salesforce-sync-settings-13.png)

1. 目的のオプションを選択します（「[!DNL Salesforce] タスクに同期しない」がデフォルトで選択されています）。

   ![](assets/salesforce-sync-settings-14.png)

## [!DNL Sales Insight Actions] タスクの [!DNL Salesforce] との初めての同期 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

[!DNL Sales Insight Actions] と [!DNL Salesforce] のタスク間の同期を初めて有効にすると、[!DNL Salesforce] のタスクが読み込まれます。[!DNL Sales Insight Actions] の現在のタスクは [!DNL Salesforce] にプッシュされません。[!DNL Sales Insight Actions] から [!DNL Salesforce] に同期されるタスクは、[!DNL Sales Insight Actions] を SFDC と同期した後に作成されるタスクのみです。

[!DNL Sales Insight Actions] と SFDC のタスクを同期すると、次の処理が行われます。

タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

過去 24 時間に更新または作成されたリマインダーは、SFDC から [!DNL Sales Insight Actions] に取り込まれます。同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

同期が有効になっている限り、[!DNL Sales Insight Actions] と SFDC の間でタスクが常に同期されます。

初回同期の後、[!DNL Sales Insight Actions] で作成、編集、完了または削除したタスクは、[!DNL Salesforce] のタスクリストに同期されます。また、[!DNL Salesforce] でタスクが作成、編集、完了、削除されると、[!DNL Sales Insight Actions] のタスクリストが更新されます。

この同期を有効にするには、web アプリケーションの[!UICONTROL 設定ページ]で同期ボックスをオンにします。
