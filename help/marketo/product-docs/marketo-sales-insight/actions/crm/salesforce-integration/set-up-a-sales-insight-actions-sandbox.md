---
description: Sales Insight アクションサンドボックスの設定 — Marketoドキュメント — 製品ドキュメント
title: Sales Insight アクションサンドボックスの設定
exl-id: 58af77ef-93ea-4149-be91-f86cdc8f7476
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 8%

---

# Sales Insight アクションサンドボックスの設定 {#set-up-a-sales-insight-actions-sandbox}

>[!NOTE]
>
>Marketo Sales Insight Actions は、[Marketo Sales Insight パッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}を使用して Salesforce ユーザーインターフェイスと統合された、web ベースのアプリケーションです。「Marketo Sales」や、シンプルに「Actions」と呼ばれることもあります。

Marketo Sandbox を持っている場合、Actions インスタンスをサンドボックスと共にテスト目的で使用できるようにします。

Actions インスタンスを設定する際は、Salesforce Sandbox と Salesforce 実稼動のどちらで動作するかを設定する必要があります。 これは、Salesforce がそれぞれ異なるエンドポイントを使用し、アクションが Salesforce への接続を使用して、ユーザーをアクティベートおよび認証するためです。

Salesforce Sandbox インスタンスと連携するように Actions インスタンスを設定するには、以下の手順に従います。

>[!NOTE]
>
>ユーザーがどのように行動するかについて詳しく知ることができます [アクションシートを有効化](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-checklist.md){target="_blank"}. You can also learn about how users will [authenticate with Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}. Additionally, if you prefer to have users authenticate with email and password, you can learn more about this in our [Login Management settings article](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

## Marketo Sandbox にプロビジョニングするアクションインスタンスのリクエスト {#request=an-actions-instance}

Marketo Sandbox インスタンスに対しては、要求されない限り Sales Insight アクションが有効になっていません。 リクエストを送信するには、Adobeアカウントチーム（担当のアカウントマネージャー）にお問い合わせください。

## Marketo Sandbox 用のアクションアカウントのプロビジョニング {#provision-your-actions-account}

Marketo Sandbox でアクションが有効になったら、以下の手順に従って新しいインスタンスをアクティブ化する必要があります。

1. Marketo Sandbox インスタンスにログインします。

1. に移動します。 **管理者**.

1. 選択 **Sales Insight**.

1. 選択 **アクション設定**.

   >[!IMPORTANT]
   >
   >電子メールアドレスは、サンドボックスインスタンスと実稼働インスタンスの両方の 1 つのアクションインスタンスに対してのみ使用できます。 実稼動環境とサンドボックス全体の複数のインスタンスにアクセスする必要がある管理者の場合は、それぞれに異なる電子メールアドレスを使用する必要があります。

1. プロビジョニングカードで、Sales Insight Actions インスタンスに招待するユーザーを選択します。

## アクションインスタンスをアクティブ化 {#activate-your-actions-instance}

アクションインスタンスは、Salesforce 本番アカウントで有効化する必要があります。 有効化した後は、Salesforce Sandbox アカウントに切り替えることができます。

1. 送信した招待を探します。

1. 次をクリック： **はじめに** リンク。

1. Salesforce 本番インスタンスでアクティブ化します。

1. 画面の指示に従ってアカウントを設定します。 詳細な概要については、 [ユーザーのオンボーディング記事](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}.

## Salesforce Sandbox インスタンスとの互換性を確保するためのアクションインスタンスの準備 {#prepare-your-actions-instance}

アクションを実行するには、まず Salesforce 実稼動ユーザーが新しいインスタンスをアクティブ化する必要があります。 有効化したら、次の手順を使用して、Salesforce Sandbox との互換性を持つインスタンスを準備できます。

1. ログイン設定を「All Login Methods」に更新し、必要に応じてユーザ名とパスワードを使用してログインできるようにします。 必要に応じて、すべてが設定された後で、「Salesforce のみ」に切り替えることができます。 [この方法については、こちらを参照してください。](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

1. Salesforce 実稼動環境から切断し、Salesforce サンドボックスに接続します。 [接続方法を見る](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}. 手順 3 では、「Salesforce」ではなく「サンドボックス」を選択します。 既に接続している場合は、「Salesforce 接続とカスタマイズ」タブで連携を解除するオプションが表示されます。

>[!NOTE]
>
>Salesforce インスタンスのカスタムドメインがある場合は、Salesforce に接続する前に Salesforce インスタンスにログインするか、Actions にログインする前に Salesforce インスタンスにログインすることをお勧めします。

## Salesforce Sandbox との互換性を持たせるためにアクションインスタンスを変換するリクエスト {#request-your-actions-instance-be-converted}

1. 連絡先 [Marketo Engageサポート](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} 新しい Sales Insight Actions インスタンスを Salesforce Sandbox との互換性を持たせるように構成するには、次の手順を実行します。

1. toutapp.com/loginページの「Salesforce でログイン」ボタンを使用してログインを試みることで、すべてが正しく設定されていることをテストします。

   ![](assets/set-up-a-sales-insight-actions-sandbox-1.png)

   >[!TIP]
   >
   >この時点で問題が発生した場合は、パスワードのリセットをリクエストし、パスワードを使用して、アカウントに再びアクセスできるようにします。

これで、インスタンスを Salesforce Sandbox インスタンスで使用する準備が整いました。 を使用したい場合 [Salesforce 自動ログイン](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"} from Salesforce, you can switch back to "Salesforce Only" in your [Login Management settings](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}.

>[!NOTE]
>
>* [Sales Insight Actions アカウントを Salesforce に接続](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md){target="_blank"}
>* [Sales Insight Actions ユーザーオンボーディングガイド](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-user-onboarding-guide.md){target="_blank"}
>* [Salesforce からの自動ログイン](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md){target="_blank"}
>* [ログイン管理の設定](/help/marketo/product-docs/marketo-sales-insight/actions/admin/login-management-settings.md){target="_blank"}
