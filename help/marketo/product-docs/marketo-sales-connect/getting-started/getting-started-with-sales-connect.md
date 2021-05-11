---
unique-page-id: 13796466
description: Sales Connectの使い始めに —Marketoドキュメント — 製品ドキュメント
title: Sales Connectの使い始めに
exl-id: 8c5b1f65-449c-4304-b904-fc6442a47e5a
translation-type: tm+mt
source-git-commit: 20ccc6ba2b26b869776ed88ed6fe76a67f74400a
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Sales Connectの使い始めに{#getting-started-with-sales-connect}

これらの手順を読むよりも見たい場合は、](#video)の下の[ビデオの手順に進んでください。

>[!AVAILABILITY]
>
>この機能を購入していないお客様もいます。 詳しくは、カスタマーサクセスマネージャーにお問い合わせください。

## 使い始めるために必要なもの{#what-you-need-to-get-started}

* Marketo購読
* Sales Connect購読
* Salesforce購読（API呼び出しとApexクラスが有効）

## 開始に必要なユーザー{#who-you-need-to-get-started}

* Marketo管理者ユーザー
* Sales Connect Adminユーザー
* Salesforce管理者
* Sales Connectユーザー

## Sales Connect管理者{#sales-connect-admins}

パスワードをリセットするためのリンクが記載された電子メールがMarketoから送信されます。 新しいパスワードを作成したら、Sales Connectにログインします。

セットアップを完了するには、次の操作を行う必要があります。

* [Sales ConnectとSalesforceの接続](#connect-your-sales-connect-account-to-salesforce)
* [Sales ConnectをMarketoに接続する前に資格情報を取得](#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo)
* [Connect Sales Connect (Marketoとの接続)](#connect-sales-connect-to-marketo)
* [ユーザーの招待/プロビジョニング](#invite-provision-users)

オプションで、次のこともできます。

* [SandboxでのSales Connectのテスト](#test-sales-connect-in-your-sandbox)

## Sales ConnectアカウントをSalesforceに接続{#connect-your-sales-connect-account-to-salesforce}

Sales ConnectアカウントをSalesforceアカウントに接続するには、管理者または非管理者として、[この記事](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)の手順に従います。

>[!NOTE]
>
>接続するSalesforceのインスタンスは、Marketoに接続されている（または接続される）のと同じインスタンスである必要があります。

## Sales ConnectをMarketoに接続する前に資格情報を取得する{#acquiring-credentials-prior-to-connecting-sales-connect-with-marketo}

Marketo内から資格情報を取得する必要があります。 これらの資格情報は、後でSales Connect管理者がMarketoとSales Connectを接続する際に使用します。

1. Marketoで、**管理者**&#x200B;をクリックします。

   ![](assets/one.png)

1. ツリーで、[**販売用接続**]をクリックします。

   ![](assets/two.png)

1. 以下のMarketo資格情報を選択し、Sales Connect管理者に送信します。Munchkin ID、Client ID、Client Secret。

   ![](assets/3.jpg)

   >[!NOTE]
   >
   >上記の情報をコピーして貼り付ける場合は、スペースが追加されていないことを確認してください。

## セールス・コネクトをMarketoに接続{#connect-sales-connect-to-marketo}

1. 「Sales Connect」で、歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/four.png)

1. 「管理設定」で、**Marketo**&#x200B;を選択します。

   ![](assets/eight.png)

1. Marketo管理者から提供されたMarketoの資格情報を入力し、**「接続**」をクリックします。

   ![](assets/credentials.png)

## ユーザーの招待/プロビジョニング{#invite-provision-users}

お客様のアカウントに既に存在するユーザー（旧称ToutApp）は、Sales Connectの「Marketo」セクションの「**チームアクセス**」タブに表示されます。

このページから、チームをMarketoのSales Connect Userとしてプロビジョニングできます。 ToutAppを初めて使用した場合や、まだユーザーを招待していない場合は、[この記事](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md)の手順に従ってください。

>[!CAUTION]
>
>Sales ConnectをMarketoに接続してから10分待ってから、これらの手順を実行してください。

1. 1人または複数のユーザーを選択し、「**接続**」をクリックします。

   >[!NOTE]
   >
   >ワークスペースの割り当ては、ユーザーを招待したときに1回だけ実行できます。 設定後は、ユーザーの接続を切断して変更する必要があります。

   ![](assets/users.png)

1. Marketo購読でワークスペースが有効になっている場合、各ユーザーまたは一連のユーザーにワークスペースを一括して割り当てることができます。 ワークスペースが選択されていない場合は、デフォルトのMarketoワークスペースに割り当てます。

   ![](assets/nine.jpg)

1. ワークスペースドロップダウンをクリックし、目的のワークスペースを選択して、**接続**&#x200B;をクリックします。

   ![](assets/ten.png)

   >[!NOTE]
   >
   >新しいユーザーを追加する場合は、管理設定の「チーム管理」セクションに移動し、「**ユーザーを招待**」ボタンをクリックします。

チームの管理ページから追加のユーザーを追加し、上記の手順に従ってユーザーを接続できます。

## SandboxでのSales Connectのテスト{#test-sales-connect-in-your-sandbox}

MarketoセールスコンネクトをMarketoサンドボックスでテストしたいチームの場合は、リクエストに応じて追加のSales Connectアカウントをプロビジョニングできます。 これは、Marketoサンドボックスを購入したお客様、またはMarketoバンドルの一部として購入したお客様向けです。 サンドボックスの取得に関心がある場合は、Marketoのアカウントマネージャーにお問い合わせください。

>[!NOTE]
>
>同じ電子メールIDを持つSales Connectアカウントを複数のインスタンスにプロビジョニングすることはできません。 つまり、追加のSales Connectアカウントを使用して、MarketoSandboxインスタンスでテストを行う場合は、各アカウントで異なる電子メールIDを使用する必要があります。
