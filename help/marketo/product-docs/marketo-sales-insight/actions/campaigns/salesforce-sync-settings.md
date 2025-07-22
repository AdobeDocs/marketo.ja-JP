---
description: Salesforce 同期設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce 同期設定
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 30%

---

# [!DNL Salesforce] Sync Settings {#salesforce-sync-settings}

## API を使用した [!DNL Salesforce] へのメールアクティビティのログ記録 {#logging-email-activity-to-salesforce-via-api}

この機能を使用するには、[!DNL Salesforce] の Enterprise/Unlimited 版、または Web サービス API 経由で統合を購入している場合は Professional 版を使用する必要があります。

>[!PREREQUISITES]
>
>[!DNL Salesforce] と [!DNL Sales Insight Actions] を接続する必要があります。

1. [!DNL Sales Insight Actions] で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/salesforce-sync-settings-1.png)

1. [!UICONTROL &#x200B; 管理者設定 &#x200B;] （管理者でない場合は「[!UICONTROL &#x200B; マイアカウント &#x200B;]」）で、**[!UICONTROL Salesforce]** をクリックします。

   ![](assets/salesforce-sync-settings-2.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/salesforce-sync-settings-3.png)

1. [!UICONTROL &#x200B; メールのアクティビティを記録 &#x200B;] の横にある矢印をクリックして [!DNL Salesforce] きます。

   ![](assets/salesforce-sync-settings-4.png)

1. 「**[!UICONTROL Salesforce API]**」タブをクリックします。このカードでは、[!DNL Salesforce] に情報を記録するための環境設定を行うことができます。 終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/salesforce-sync-settings-5.png)

## [!DNL Salesforce] へのメール（BCC）経由での [!DNL Salesforce] へのメールアクティビティのログ記録 {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

「[!UICONTROL Salesforceにメールを送信（BCC） &#x200B;]」を有効化すると、営業メールの BCC が送信されます。メールは、商談、リードおよび連絡先のアクティビティとして記録されます。

>[!PREREQUISITES]
>
>[!DNL Salesforce] と [!DNL Sales Insight Actions] を接続する必要があります。

**メール（BCC）で [!DNL Salesforce] にメールを記録するには**

1. Marketo Sales で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/salesforce-sync-settings-6.png)

1. [!UICONTROL &#x200B; 管理者設定 &#x200B;] （管理者でない場合は「[!UICONTROL &#x200B; マイアカウント &#x200B;]」）で、**[!UICONTROL Salesforce]** をクリックします。

   ![](assets/salesforce-sync-settings-7.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/salesforce-sync-settings-8.png)

1. 「**[!UICONTROL Salesforce にメールを送信（BCC）]**」タブをクリックし、「**[!UICONTROL 有効化]**」をクリックします。

   ![](assets/salesforce-sync-settings-9.png)

何らかの理由で [!DNL Salesforce] アドレスへのメールが取り込まれない場合は、次の手順に従って、[!DNL Salesforce] アカウントで BCC 機能を有効にします。

1. [!DNL Salesforce] インスタンスにログインします。
1. 右上隅にあるユーザー名を探し、ドロップダウンバーを選択します。
1. 「**[!UICONTROL マイ設定]**」を選択します。
1. 「**[!UICONTROL メール]**」を選択します。
1. 「**[!UICONTROL メールを Salesforce に送信]**」を選択します。
1. このページには、「[!UICONTROL Salesforce アドレスにメールを送信 &#x200B;]」というラベルの付いたフィールドが表示されます。 その横に何も入力されていない場合は、下にスクロールして「[!UICONTROL &#x200B; 使用可能なメールアドレス &#x200B;]」を表示します。
1. BCC を送信するメールアドレスを入力します。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

**設定に [!DNL Salesforce] するメールが見つかりません**

「設定」の下に「[!DNL Salesforce] へのマイメール」が表示されない場合は、管理者が有効にしていない可能性があります。 これは、チームが [!DNL Salesforce] を初めて使用する場合や、チームが [!DNL Salesforce] から提供された BCC アドレスを使用したことがない場合に発生する可能性があります。

>[!NOTE]
>
>これを設定するには、管理者権限が必要です。

1. 「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL メール管理]**」をクリックします。
1. 「**[!UICONTROL Salesforce にメール送信]**」をクリックします。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. 「アクティブ」の横のボックスをオンにします。
1. 「**[!UICONTROL 保存]**」をクリックします。

## [!DNL Sales Insight Actions] のタスク/リマインダーを [!DNL Salesforce] のタスクに同期 {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. [!DNL Sales Insight Actions] で、歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/salesforce-sync-settings-10.png)

1. [!UICONTROL &#x200B; 管理者設定 &#x200B;] （管理者でない場合は「[!UICONTROL &#x200B; マイアカウント &#x200B;]」）で、**[!UICONTROL Salesforce]** をクリックします。

   ![](assets/salesforce-sync-settings-11.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/salesforce-sync-settings-12.png)

1. 「Marketo Sales Tasks/Reminders to [!DNL Salesforce] Tasks」の横の矢印をクリックします。

   ![](assets/salesforce-sync-settings-13.png)

1. 目的のオプションを選択します（「[!DNL Salesforce] のタスクに同期しない」はデフォルトで選択されています）。

   ![](assets/salesforce-sync-settings-14.png)

## [!DNL Sales Insight Actions] タスクの [!DNL Salesforce] との初めての同期 {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

最初に [!DNL Sales Insight Actions] タスクと [!DNL Salesforce] タスクの同期を有効にすると、[!DNL Salesforce] タスクがインポートされます。 お客様が現在のタスクをプッシ [!DNL Sales Insight Actions] で完了できるよ [!DNL Salesforce] には、進めません。 煩雑さと重複を減らすために、[!DNL Sales Insight Actions] から [!DNL Salesforce] に同期されるタスクは、SFDCと同期した後に作成されるタスクのみ [!DNL Sales Insight Actions] す。

[!DNL Sales Insight Actions] タスクとSFDC タスクを同期すると、次のようになります。

タスクの同期で「保存」をクリックすると、タスクの同期が開始されます。最初は時間がかかります。

過去 24 時間以内に更新または作成されたリマインダーは、SFDCから [!DNL Sales Insight Actions] に取り込まれます。 同期は期限に基づいており、これらのタスクはすべてバックエンドで同期されますが、コマンドセンターでは、今日と明日のタスクのみが表示されます。

同期が以前にオンになっていて、SFDC 内のタスクを削除した場合、過去 15 日間に削除されたすべてのタスクがコマンドセンターから削除されます。

同期が有効になっている限り、[!DNL Sales Insight Actions] とSFDCの間でタスクを継続的に同期します。

最初の同期の後、[!DNL Sales Insight Actions] で作成、編集、完了または削除したタスクは、[!DNL Salesforce] のタスクリストに同期されます。 [!DNL Salesforce] で作成、編集、完了または削除すると、[!DNL Sales Insight Actions] のタスクリストが更新されます。

この同期を有効にするには、web アプリケーションの [!UICONTROL &#x200B; 設定 &#x200B;] ページで「同期」ボックスをオンにするだけです。
