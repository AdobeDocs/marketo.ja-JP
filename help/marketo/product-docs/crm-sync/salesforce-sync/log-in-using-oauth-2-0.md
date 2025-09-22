---
description: OAuth 2.0 を使用したログイン - Marketo ドキュメント - 製品ドキュメント
title: OAuth 2.0 を使用したログイン
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 97%

---

# OAuth 2.0 を使用したログイン {#log-in-using-oauth-2-0}

Salesforce は、OAuth プロトコルを使用して、アプリケーションのユーザがログイン資格情報を表示することなく、アプリケーションのデータに安全にアクセス（OAuth 2.0 を使用してアプリケーションを認証）できるようにします。以下は、Salesforce と安全に接続し、Marketo Engageを同期するために実行する手順です。

>[!IMPORTANT]
>
>OAuth を使用して Marketo と [!DNL Salesforce] に接続するには、誤ったユーザ名で [!DNL Salesforce] に接続しないよう、プライベート（匿名）ブラウザーで Marketo にログインします。

## 接続アプリの設定 {#set-up-connected-app}

1. Salesforce の「設定」で、プラットフォームツール内で「アプリ」、「アプリマネージャー」の順に移動し、「**[!UICONTROL 新しい接続済みアプリ]**」をクリックします。

   ![](assets/setting-up-oauth-2-1.png)

1. 詳細を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/setting-up-oauth-2-2.png)

1. 「**[!UICONTROL OAuth 設定を有効にする]**」チェックボックスをクリックします。「コールバック URL」に `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect` と入力します。使用可能なすべての OAuth 範囲を選択し、**[!UICONTROL 追加]**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-3.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/setting-up-oauth-2-4.png)

1. 「**[!UICONTROL 続行]**」をクリックします。

   ![](assets/setting-up-oauth-2-5.png)

1. 消費者キーと消費者秘密鍵をコピーします ( 後で、それらをMarketo Engageで使用するために必要になります )。

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>セットアップに干渉するので、New Connected App ページを表示している間に、下にスクロールして、「Require Proof Key for Code Exchange (PKCE)」チェックボックスが&#x200B;_オフ_&#x200B;になっていることを確認します。

## Marketo の設定 {#set-up-marketo}

>[!PREREQUISITES]
>
>* Salesforce 同期ユーザに対して API アクセスを有効にする必要があります（Salesforce Professional Edition ユーザの場合、そのアクセスはデフォルトでは使用できません。Salesforce アカウント担当者にお問い合わせください）。
>* Marketo 同期ユーザを Salesforce で作成する必要があります。
>* 既存の顧客の場合、顧客のサブスクリプションで「SFDC 同期で OAuth を有効にする」機能が有効になります。
>* ポップアップブロッカーが無効になっています。
>* Connected App が作成され、[!UICONTROL Consumer Key] と [!UICONTROL Consumer Secret] を使用できるようになりました。

>[!CAUTION]
>
>同期ユーザから Marketo で不要なフィールドをすべて非表示にした後で、「**[!UICONTROL 同期フィールド]**」をクリックするようにしてください。「同期フィールド」をクリックすると、ユーザが SFDC で表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. Marketo の管理セクションで、**[!UICONTROL CRM]**／**[!UICONTROL Salesforce と同期]**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-7.png)

1. 以前に記録した Consumer Key および Consumer Secret の情報を追加し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/setting-up-oauth-2-8.png)

1. Marketo Salesforce 同期ページで、「**[!UICONTROL Salesforce でログイン]**」ボタンをクリックします。

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >「Salesforce でログイン」ボタンではなく、「ユーザー名」、「パスワード」、「トークン」の各フィールドが表示されている場合は、Marketo サブスクリプションの基本認証が有効になっています。詳しくは、[基本認証を使用した Marketo の設定](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}を参照してください。同期が一連の資格情報を使用し始めると、Salesforce の資格情報またはサブスクリプションを切り替えられなくなります。Salesforce認証用に Oauth 2.0 を設定するには、[Marketo サポート ](https://nation.marketo.com/t5/support/ct-p/Support) にお問い合わせください。

1. Salesforce ログインページのポップアップが表示されます。「Marketo 同期ユーザー」資格情報をキー入力し、ログインします。

   ![](assets/setting-up-oauth-2-10.png)

1. メールで受け取った検証コード（Salesforce から送信）を入力し、**[!UICONTROL 検証]**&#x200B;をクリックします。

   ![](assets/setting-up-oauth-2-11.png)

1. 検証が成功すると、アクセスをリクエストするアクセスページが表示されいます。「**[!UICONTROL 許可]**」をクリックします。

   ![](assets/setting-up-oauth-2-12.png)

1. 数分後に、Marketo にポップアップが表示されます。「**[!UICONTROL 資格情報を確認]**」をクリックします。

   ![](assets/setting-up-oauth-2-13.png)

1. フィールドの同期が完了したら、「**[!UICONTROL Salesforce 同期を開始]**」をクリックします。

   ![](assets/setting-up-oauth-2-14.png)

1. 「**[!UICONTROL 同期の開始]**」をクリックします。

   ![](assets/setting-up-oauth-2-15.png)

Marketo と [!DNL Salesforce] の同期が進行中です。

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [手順 2 / 3：Marketo 用の Salesforce ユーザの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Salesforce AppExchange での Marketo セールスインサイトパッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Salesforce Enterprise／Unlimited での Marketo セールスインサイトの設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
