---
unique-page-id: 18317669
description: Salesforce 同期設定 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce 同期設定
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 100%

---

# Salesforce 同期設定 {#salesforce-sync-settings}

## メールアクティビティのログを API 経由で Salesforce に記録 {#logging-email-activity-to-salesforce-via-api}

この機能を使用するには、Salesforce の Enterprise／Unlimited エディション、または web サービス API を通じて統合を購入済みの場合は Professional エディションを使用する必要があります。

>[!PREREQUISITES]
>
>Salesforce と Sales Connect を接続する必要があります。

1. [!DNL Sales Connect] で、右上の歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one-2.png)

1. 「[!UICONTROL マイアカウント]」（管理者の場合は[!UICONTROL 管理者設定]）で、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/two-2.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/three-1.png)

1. 「メールアクティビティのログを [!DNL Salesforce] に記録」の横の矢印をクリックします。

   ![](assets/four-1.png)

1. 「**[!UICONTROL Salesforce API]**」タブをクリックします。このカードでは、[!DNL Salesforce] に情報を記録する際の環境設定を設定できます。終了したら「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/five.png)

## メールアクティビティのログを Salesforce にメール送信（BCC）して Salesforce に記録 {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

「Salesforce にメールを送信（BCC）」を有効にすると、セールスメールの BCC が送信され、メールは商談、リード、取引先責任者に関するアクティビティとして記録されます。

>[!PREREQUISITES]
>
>[!DNL Salesforce] および [!DNL Sales Connect] を接続する必要があります。

**メール（BCC）を使用して Salesforce にメールを記録するには**

1. [!UICONTROL Sales Connect] で、右上の歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one-3.png)

1. 「[!UICONTROL マイアカウント]」（管理者の場合は[!UICONTROL 管理者設定]）で、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/two-3.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/three-1.png)

1. 「**[!UICONTROL Salesforce にメールを送信（BCC）]**」タブをクリックし、「**[!UICONTROL 有効化]**」をクリックします。

   ![](assets/six-2.png)

何らかの理由で [!DNL Salesforce] へのメールアドレスが取り込まれない場合は、以下の手順に従って、[!DNL Salesforce] アカウントで BCC 機能を有効にします。

1. [!DNL Salesforce] インスタンスにログインします。
1. 右上隅にあるユーザー名を探し、ドロップダウンバーを選択します。
1. 「**[!UICONTROL マイ設定]**」を選択します。
1. 「**[!UICONTROL メール]**」を選択します。
1. 「**[!UICONTROL メールを Salesforce に送信]**」を選択します。
1. このページに、「Salesforce アドレス宛てにメールを送信」というラベルの付いたフィールドが表示されます。横に何も入力されていない場合は、「アクセス可能なメールアドレス」までスクロールします。
1. BCC を送信するメールアドレスを入力します。
1. 「**[!UICONTROL 変更を保存]**」をクリックします。

**マイ設定で [!DNL Salesforce] へのメール送信が見つからない**

「設定」に「Salesforce へのメール送信」が表示されない場合は、管理者が有効にしていない可能性があります。これは、チームが [!DNL Salesforce] を初めて使用した場合や、チームが [!DNL Salesforce] が提供する BCC アドレスを使用したことがない場合に発生する可能性があります。

>[!NOTE]
>
>これを設定するには、管理者権限が必要です。

1. 「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL メール管理]**」をクリックします。
1. 「**[!UICONTROL Salesforce にメール送信]**」をクリックします。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. 「[!UICONTROL アクティブ]」の横のボックスをオンにします。
1. 「**[!UICONTROL 保存]**」をクリックします。

## Sales Connect タスク／[!DNL Salesforce] タスクのリマインダーを同期 {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. 右上の歯車アイコンをクリックし、「**[!UICONTROL 設定]**」を選択します。

   ![](assets/one-3.png)

1. 「[!UICONTROL マイアカウント]」（管理者の場合は[!UICONTROL 管理者設定]）で、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/two-2.png)

1. 「**[!UICONTROL 同期設定]**」タブをクリックします。

   ![](assets/three-1.png)

1. 「[!UICONTROL Sales Engage タスク／Salesforce タスクのリマインダーを同期]」の横の矢印をクリックします。

   ![](assets/seven-2.png)

1. 目的のオプションを選択します（「[!UICONTROL Salesforce タスクに同期しない]」がデフォルトで選択されています）。

   ![](assets/eight.png)
