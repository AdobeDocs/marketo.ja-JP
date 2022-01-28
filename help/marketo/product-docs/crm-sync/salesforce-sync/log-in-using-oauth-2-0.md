---
description: OAuth 2.0 を使用してログインする — Marketoドキュメント — 製品ドキュメント
title: OAuth 2.0 を使用したログイン
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
source-git-commit: c15753e0f2af199af8fd7e8bfe0924a915a39814
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 9%

---

# OAuth 2.0 を使用したログイン {#log-in-using-oauth-2-0}

Salesforce は、OAuth プロトコルを使用して、アプリケーションのユーザーがログイン資格情報を表示することなく、アプリケーションのデータに安全にアクセス（OAuth 2.0 を使用してアプリケーションを認証）できるようにします。 Marketoを Salesforce と安全に接続し、同期するために実行する手順を以下に示します。

>[!IMPORTANT]
>
>OAuth を使用してMarketoと Salesforce に接続するには、誤ったユーザー名で Salesforce に接続しないよう、プライベート（匿名）ブラウザーでMarketoにログインします。

## 接続アプリのセットアップ {#set-up-connected-app}

1. Salesforce の「設定」で、プラットフォームツール内の「アプリ」、「アプリマネージャー」の順に移動し、 **新しい接続済みアプリ**.

   ![](assets/setting-up-oauth-2-1.png)

1. 詳細を入力し、 **保存**.

   ![](assets/setting-up-oauth-2-2.png)

1. 次をクリック： **OAuth 設定を有効にする** チェックボックス。 「コールバック URL」に、と入力します。 `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. 使用可能なすべての OAuth 範囲を選択し、 **追加**.

   ![](assets/setting-up-oauth-2-3.png)

1. 「**保存**」をクリックします。

   ![](assets/setting-up-oauth-2-4.png)

1. クリック **続行**.

   ![](assets/setting-up-oauth-2-5.png)

1. 消費者キーと消費者秘密鍵をコピーします。

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>後でMarketoで使用するために、消費者キーおよび消費者秘密鍵の情報を保存します。

## Marketoの設定 {#set-up-marketo}

>[!PREREQUISITES]
>
>* Salesforce 同期ユーザに対して API アクセスを有効にする必要があります（Salesforce Professional Edition ユーザの場合、そのアクセスはデフォルトでは使用できません。Salesforce アカウント担当者にお問い合わせください）。
>* Marketo同期ユーザは Salesforce で作成する必要があります。
>* 既存のお客様の場合、顧客のサブスクリプションで「OAuth for SFDC 同期を有効にする」機能が有効になります。
>* ポップアップブロッカーが無効になっています。
>* Connected App が作成され、Consumer Key と Consumer Secret を使用できるようになりました。


>[!CAUTION]
>
>同期ユーザーがMarketoで必要としないすべてのフィールドを非表示にしてから、 **フィールドを同期**. 「フィールドを同期」をクリックすると、SFDC でユーザーに表示されるすべてのフィールドがMarketoに永久に作成され、削除できなくなります。

1. 「 Marketo Admin 」セクションで、 **CRM**&#x200B;を、 **Salesforce と同期**.

   ![](assets/setting-up-oauth-2-7.png)

1. 以前に記録した消費者キーおよび消費者秘密鍵の情報を追加し、「 」をクリックして、 **保存**.

   ![](assets/setting-up-oauth-2-8.png)

1. Marketo Salesforce 同期ページで、 **Salesforce でログイン** 」ボタンをクリックします。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >「Salesforce でログイン」ボタンではなく、「ユーザー名」、「パスワード」、「トークン」の各フィールドが表示されている場合は、Marketoサブスクリプションが基本認証で有効になっています。 詳しくは、 [基本認証を使用したMarketoのセットアップ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). 一連の資格情報を使用して同期が開始されると、Salesforce の資格情報や購読は切り替えられません。 OAuth 2.0 を使用する場合は、カスタマーサクセスマネージャーにお問い合わせください。

1. Salesforce ログインページのポップアップが表示されます。 「Marketo同期ユーザー」資格情報をキーで入力し、ログインします。

   ![](assets/setting-up-oauth-2-10.png)

1. 受け取った検証コード（Salesforce から送信）を入力し、 **検証**.

   ![](assets/setting-up-oauth-2-11.png)

1. 検証が成功すると、アクセスページが表示され、アクセスをリクエストしています。 クリック **許可**.

   ![](assets/setting-up-oauth-2-12.png)

1. 数分後に、Marketoにポップアップが表示されます。 クリック **認証情報の確認**.

   ![](assets/setting-up-oauth-2-13.png)

1. フィールドの同期が完了したら、 **Salesforce 同期の開始**.

   ![](assets/setting-up-oauth-2-14.png)

1. 「**同期の開始**」をクリックします。

   ![](assets/setting-up-oauth-2-15.png)

Marketoと Salesforce の同期が進行中です。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [手順 1 / 3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順 2 / 3：Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

