---
description: OAuth 2.0の設定 — Marketto Docs — 製品ドキュメント
title: OAuth 2.0のセットアップ
translation-type: tm+mt
source-git-commit: 2d03d93e120c8b3ce359c6aca44730cfa7c16bf9
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# OAuth 2.0のセットアップ{#setting-up-oauth-2-0}

SalesforceはOAuthプロトコルを使用して、アプリケーションのユーザーが、ログイン資格情報を明らかにすることなく、REST API呼び出しを介して安全にデータにアクセス（OAuth 2.0を使用してアプリケーションを認証）できるようにします。 以下は、MarketoとSalesforceとの安全な接続と同期を行うための手順です。

## 接続されたアプリのセットアップ{#set-up-connected-app}

1. Salesforceの「設定」で、プラットフォームツール内の「アプリ」、「アプリマネージャー」に移動し、「**新しく接続されたアプリ**」をクリックします。

   ![](assets/setting-up-oauth-2-1.png)

1. 詳細を入力し、「**保存**」をクリックします。

   ![](assets/setting-up-oauth-2-2.png)

1. 「**OAuth設定を有効にする**」チェックボックスをクリックします。 コールバックURLには、`https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`と入力します。 使用可能なすべてのOAuthスコープを選択し、**追加**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-3.png)

1. 「**保存**」をクリックします。

   ![](assets/setting-up-oauth-2-4.png)

1. 「**続行**」をクリックします。

   ![](assets/setting-up-oauth-2-5.png)

1. Consumer keyとConsumer secretをコピーします。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Consumer keyとConsumer secretの情報を保存して、Marketoで後で使用できるようにします。

## マーケティングの設定{#set-up-marketo}

>[!PREREQUISITES]
>
>* Salesforce Sync Userに対してAPIアクセスを有効にする必要があります（Salesforce Professional Editionユーザの場合、そのアクセスはデフォルトでは使用できません。Salesforceアカウント担当者にお問い合わせください）。
>* Marketo SyncユーザーはSalesforceで作成する必要があります。
>* 既存のお客様の場合、お客様の購読で「OAuth for SFDCの同期を有効にする」機能が有効になります。
>* ポップアップブロッカーは無効です。
>* 接続されたアプリが作成され、Consumer keyとConsumer secretが使用可能になります。


1. 「Marketo Admin」セクションで、**CRM**&#x200B;をクリックし、**Salesforce**&#x200B;と同期をクリックします。

   ![](assets/setting-up-oauth-2-7.png)

1. 追加前に記録したConsumer keyとConsumer secretの情報をクリックし、「**保存**」をクリックします。

   ![](assets/setting-up-oauth-2-8.png)

1. Marketo Salesforceの同期ページで、「**Salesforce**&#x200B;にログイン」ボタンをクリックします。

   ![](assets/setting-up-oauth-2-9.png)

1. salesforceログインページのポップアップが表示されます。 「マーケティングツールの同期ユーザー」資格情報をキー入力し、ログインします。

   ![](assets/setting-up-oauth-2-10.png)

1. 電子メールで受け取った検証コード（Salesforceから送信）を入力し、「**検証**」をクリックします。

   ![](assets/setting-up-oauth-2-11.png)

1. 検証に成功すると、アクセスページが表示され、アクセスを要求しています。 「**許可**」をクリックします。

   ![](assets/setting-up-oauth-2-12.png)

1. 数分後に、Marketoにポップアップが表示されます。 「**資格情報を確認**」をクリックします。

   ![](assets/setting-up-oauth-2-13.png)

1. フィールドの同期が完了したら、**開始Salesforce同期**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-14.png)

1. **開始同期**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-15.png)

MarketoとSalesforceの同期が進行中です。

![](assets/setting-up-oauth-2-16.png)
