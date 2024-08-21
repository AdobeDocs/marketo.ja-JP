---
description: Sales Insight Actions サンドボックスの設定 - Marketo ドキュメント - 製品ドキュメント
title: Sales Insight Actions サンドボックスの設定
exl-id: 8bc3a8a6-7fbc-4cbe-99a7-21b066ec4f96
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: ht
source-wordcount: '671'
ht-degree: 100%

---

# Sales Insight Actions サンドボックスの設定 {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions は、[Marketo Sales Insight パッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}を使用して Salesforce CRM と排他的に統合された、web ベースのアプリケーションです。「Marketo Sales」や、シンプルに「Actions」と呼ばれることもあります。

Marketo サンドボックスがある場合、Actions インスタンスを、テスト目的でサンドボックスと共に使用できるようにすることができます。

Actions インスタンスを設定する場合、Salesforce サンドボックスと連携するように設定するか、Salesforce 実稼動と連携するように設定するかを決定する必要があります。これは、Salesforce ではそれぞれに対し異なるエンドポイントを使用し、Actions ではユーザのアクティブ化と認証に Salesforce への接続を使用するからです。

Salesforce サンドボックスインスタンスと連携するように Actions インスタンスを設定するには、以下の手順に従います。

>[!NOTE]
>
>詳しくは、ユーザが [Actions シートをアクティブ化](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}する方法を参照してください。また、ユーザが [Salesforce を使用して認証](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}する方法も参照してください。さらに、ユーザにメールとパスワードによる認証を行わせる場合について詳しくは、[ログイン管理の設定の記事](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}を参照してください。

## Marketo サンドボックス にプロビジョニングする Actions インスタンスをリクエスト {#request=an-actions-instance}

Marketo サンドボックスインスタンスでは、リクエストがない限り、Sales Insight Actions が有効になりません。リクエストを送信するには、アドビのアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

## Marketo サンドボックスの Actions アカウントをプロビジョニング {#provision-your-actions-account}

Marketo サンドボックスで Actions を有効にすると、以下の手順に従って新しいインスタンスをアクティブ化する必要があります。

1. Marketo サンドボックスインスタンスにログインします。

1. **管理者**&#x200B;に移動します。

1. 「**Sales Insight**」を選択します。

1. 「**Actions の設定**」を選択します。

   >[!IMPORTANT]
   >
   >メールアドレスは、サンドボックスインスタンスと実稼動インスタンスの両方で、1 つの Actions インスタンスにのみ使用できます。管理者が実稼動環境とサンドボックス全体の複数のインスタンスにアクセスする必要がある場合は、それぞれに異なるメールアドレスを使用する必要があります。

1. プロビジョニングカードで、Sales Insight Actions インスタンスに招待するユーザを選択します。

## Actions インスタンスをアクティブ化 {#activate-your-actions-instance}

Actions インスタンスは、Salesforce 実稼動アカウントでアクティブ化する必要があります。アクティブ化したら、Salesforce サンドボックスアカウントに切り替えることができます。

1. 送信された招待を見つけます。

1. **使用を開始**&#x200B;リンクをクリックします。

1. Salesforce 実稼動インスタンスでアクティブ化します。

1. プロンプトの指示に従ってアカウントを設定します。概要について詳しくは、[ユーザのオンボーディングに関する記事](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}を参照してください。

## Salesforce サンドボックスインスタンスと互換性のある Actions インスタンスを準備 {#prepare-your-actions-instance}

Actions では、まず Salesforce の実稼動ユーザで新しいインスタンスをアクティブ化する必要があります。アクティブ化したら、次の手順に従ってインスタンスを Salesforce サンドボックスと互換性のあるものに準備できます。

1. ログイン設定を「すべてのログイン方法」に更新して、必要に応じてユーザ名とパスワードでログインできるようにします。必要に応じて、すべてを設定した後に、これを「Salesforce のみ」に戻すことができます。[その方法について詳しくは、こちらを参照してください](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}。

1. Salesforce 実稼動環境から切断し、Salesforce サンドボックスに接続します。[接続方法について詳しくは、こちらを参照してください](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}。手順 3 では、「Salesforce」ではなく「サンドボックス」を選択します。既に接続している場合は、Salesforce の「接続とカスタマイズ」タブに切断するオプションが表示されます。

>[!NOTE]
>
>Salesforce インスタンスにカスタムドメインがある場合は、Salesforce に接続する前や、Actions にログインする前に、Salesforce インスタンスにログインすることをお勧めします。

## Salesforce サンドボックスとの互換性を持たせるように Actions インスタンスの変換をリクエスト {#request-your-actions-instance-be-converted}

1. [Marketo Engage サポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}に問い合わせ、新しい Sales Insight Actions インスタンスを Salesforce サンドボックスと互換性を持たせる設定を行うようリクエストします。

1. toutapp.com/login ページの「Salesforce でログイン」ボタンを使用してログインし、すべてが正しく設定されていることをテストします。

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >この時点で問題が発生した場合は、パスワードのリセットをリクエストし、パスワードを使用してアカウントに再度アクセスできます。

これで、インスタンスを Salesforce サンドボックスインスタンスで使用する準備が整いました。Salesforce から [Salesforce 自動ログイン](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}を使用する場合は、[ログイン管理の設定](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}で「Salesforce のみ」に切り替えることができます。

>[!NOTE]
>
>* [Sales Insight Actions アカウントを Salesforce に接続](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Sales Insight Actions ユーザオンボーディングガイド](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Salesforce からの自動ログイン](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [ログイン管理の設定](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
