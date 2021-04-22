---
description: OAuth 2.0のセットアップ —Marketoドキュメント — 製品ドキュメント
title: OAuth 2.0のセットアップ
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# OAuth 2.0のセットアップ{#setting-up-oauth-2-0}

SalesforceはOAuthプロトコルを使用して、アプリケーションのユーザーが、ログイン資格情報を明らかにすることなく、REST API呼び出しを介して安全にデータにアクセス（OAuth 2.0を使用してアプリケーションを認証）できるようにします。 以下は、MarketoとSalesforceを安全に接続し、同期するために実行する手順です。

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
>後でMarketoで使用するために、Consumer keyとConsumer secretの情報を保存します。

## Marketoのセットアップ{#set-up-marketo}

>[!PREREQUISITES]
>
>* Salesforce Sync Userに対してAPIアクセスを有効にする必要があります（Salesforce Professional Editionユーザの場合、そのアクセスはデフォルトでは使用できません。Salesforceアカウント担当者にお問い合わせください）。
>* SalesforceでMarketo同期ユーザーを作成する必要があります。
>* 既存のお客様の場合、お客様の購読で「OAuth for SFDCの同期を有効にする」機能が有効になります。
>* ポップアップブロッカーは無効です。
>* 接続されたアプリが作成され、Consumer keyとConsumer secretが使用可能になります。


1. 「Marketo管理者」セクションで、「**CRM**」をクリックし、「**Salesforceと同期**」をクリックします。

   ![](assets/setting-up-oauth-2-7.png)

1. 追加前に記録したConsumer keyとConsumer secretの情報をクリックし、「**保存**」をクリックします。

   ![](assets/setting-up-oauth-2-8.png)

1. MarketoのSalesforceの同期ページで、「**Login with Salesforce**」ボタンをクリックします。

   ![](assets/setting-up-oauth-2-9.png)

1. salesforceログインページのポップアップが表示されます。 「Marketo同期ユーザー」資格情報をキー入力し、ログインします。

   ![](assets/setting-up-oauth-2-10.png)

1. 電子メールで受け取った検証コード（Salesforceから送信）を入力し、「**検証**」をクリックします。

   ![](assets/setting-up-oauth-2-11.png)

1. 検証に成功すると、アクセスページが表示され、アクセスを要求しています。 「**許可**」をクリックします。

   ![](assets/setting-up-oauth-2-12.png)

1. 数分後、Marketoにポップアップが表示されます。 「**資格情報を確認**」をクリックします。

   ![](assets/setting-up-oauth-2-13.png)

1. フィールドの同期が完了したら、**開始Salesforce同期**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-14.png)

1. **開始同期**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-15.png)

MarketoとSalesforceの同期が進行中です。

![](assets/setting-up-oauth-2-16.png)
