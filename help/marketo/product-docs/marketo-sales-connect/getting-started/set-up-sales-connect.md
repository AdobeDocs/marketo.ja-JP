---
description: Sales Connectの設定 —Marketoドキュメント — 製品ドキュメント
title: Sales Connectの設定
source-git-commit: 89d46ccadabec8c4dbc2db3cd9cde705c95b3978
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Sales Connectのセットアップ{#set-up-sales-connect}

このドキュメントでは、新しいSales Connectインスタンスを設定するための最初の手順を説明します。 これらの手順の一部では、Marketo管理者、Salesforce管理者、Sales Connect管理者としてアクセスする必要があります。 以下のガイドに従って、インスタンスの設定を完了します。

>[!NOTE]
>
>**管理者権限が必要です。**

## 新しいMarketoセールスコネクトアカウントにアクセス{#accessing-your-new-marketo-sales-connect-account}

Marketoセールスコネクトを購入した場合は、Marketoの管理セクションからインスタンスへのアクセスがプロビジョニングされます。 [ここをクリック](/help/marketo/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance.md) すると、Marketo管理者が新しいインスタンスへのアクセスをプロビジョニングする方法に関する手順が表示されます。

![](assets/set-up-sales-connect-1.png)

## ユーザーの招待と管理{#inviting-and-managing-users}

MarketoからMarketoセールスコネクトアカウントをプロビジョニングし、最初の管理者ユーザーを招待したら、その管理者ユーザーはMarketoセールスコネクトユーザー管理ページから別のユーザーを招待できます。 [ここをクリック](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) して、ユーザー管理ページからユーザーを招待する方法を確認します。

![](assets/set-up-sales-connect-2.png)

## Salesforceに接続中{#connecting-to-salesforce}

電子メール、呼び出し、タスクなどの販売員に対してログ販売アクティビティを有効にするには、すべてのユーザがSalesforceに個別に接続する必要があります。 ただし、管理者としてSalesforceに接続すると、チーム全体に対してアクティビティログの設定を構成できるので、すべてのSales Connectユーザーにグローバルログの設定が適用されます。

Sales ConnectインスタンスをSalesforceインスタンスに、管理者または非管理者として接続するには、[この記事](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)の手順に従います。

![](assets/set-up-sales-connect-3.png)

## Marketoに接続中{#connecting-to-marketo}

Marketoに接続すると、販売業者は自動マーケティングとマーケティングの洞察を利用して、試掘活動を行うことができます。 以下の機能を使用するには、Marketoとの統合を設定する必要があります。

* 販売業者と[マーケティングキャンペーン](/help/marketo/product-docs/marketo-sales-connect/marketo/make-a-campaign-visible-to-sales-connect-users.md)を共有
* ライブフィードに[注目の瞬間](/help/marketo/product-docs/marketo-sales-connect/marketo/interesting-moments-in-msc.md)をプッシュ
* 販売アクティビティをMarketoに記録する

Marketoに接続し、販売ユーザーにこの接続へのアクセスを許可する方法の詳細については、ここをクリックしてください。

## Salesforceカスタマイズパッケージのインストール{#installing-salesforce-customization-package}

成功のために販売を確実に行うことの一部は、主要なワークスペースに適切な機能を持つことを意味します。 Sales Connectカスタマイズパッケージを使用すると、エンゲージメント機能と主要な販売アクティビティ属性をSalesforceからアクセスできます。

Sales Connectのカスタマイズ[のインストールの詳細については、ここ](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)をクリックしてください。

## サンドボックスでのテスト{#testing-in-sandbox}

MarketoセールスコンネクトをMarketoサンドボックスでテストしたいチームの場合は、リクエストに応じて追加のSales Connectアカウントをプロビジョニングできます。 これは、Marketoサンドボックスを購入したお客様、またはMarketoバンドルの一部として購入したお客様向けです。 サンドボックスの取得に関心がある場合は、Marketoのアカウントマネージャーにお問い合わせください。

>[!NOTE]
>
>同じ電子メールIDを持つSales Connectアカウントを複数のインスタンスにプロビジョニングすることはできません。 つまり、追加のSales Connectアカウントを使用してMarketoSandboxインスタンスでテストを行う場合は、各アカウントで異なる電子メールIDを使用する必要があります。

>[!MORELIKETHIS]
[管理者権限](/help/marketo/product-docs/marketo-sales-connect/admin/user-access-details.md)>
>
