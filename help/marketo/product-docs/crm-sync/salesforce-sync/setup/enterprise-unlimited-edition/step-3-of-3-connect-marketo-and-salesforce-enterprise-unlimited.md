---
unique-page-id: 2360366
description: 手順3/3 - MarkettoとSalesforceの接続(Enterprise/Unlimited) - Marketto Docs — 製品ドキュメント
title: 手順3/3 - MarkettoとSalesforceの接続(Enterprise/Unlimited)
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---


# 手順3/3:MarketoとSalesforceの連携(Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、設定したSalesforceインスタンスと同期するようにMarketoを設定します。

>[!NOTE]
>
>**前提条件**
>
>* [手順1/3:Salesforce追加に対するマーケティング担当者のフィールド(Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順2/3:Marketor向けSalesforceユーザーの作成(Enterprise/Unlimited)](../../../../../product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) [](https://community.marketo.com/MarketoTutorial?id=kA250000000Kz5rCAC)

>



## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンをお持ちの場合は、準備のために「同期ユーザー資格情報とKDを設定」に直接進みます。

1. Marketo Syncユーザーを使用してSalesforceにログインし、同期ユーザーの名前をクリックして、「 **マイ設定**」をクリックします。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. クイック検索で「reset」と入力し、「 **Reset My Security Token**」をクリックします。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 「セキュリティトークン **のリセット**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   セキュリティトークンは電子メールで送信されます。

## 同期ユーザー資格情報の設定 {#set-sync-user-credentials}

1. Marketoで、 **Admin**( **管理者)に移動し、「** CRM **」を選択し、「 [Salesforce.comと同期」をクリックします。](http://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**Reminder**
   >
   >
   >「フィールドを [同期」をクリックする前に](../../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) 、同期ユーザーからMarketorで必要としないすべてのフィールドを必ず **非表示にしてください**。 「フィールドを同期」をクリックすると、ユーザーに表示されるすべてのフィールドが、Marketorに永久的に作成され、削除できません。

1. Salesforce設定のパート2で作成したSalesforce同期ユーザ資格情報を入力し([Professional](https://community.marketo.com/MarketoArticle?id=kA050000000LJ3QCAW)、 [Enterprise](https://community.marketo.com/MarketoArticle?id=kA050000000LIwKCAW))、「フィールドを **同期**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marketing SandboxをSalesforce Sandboxに同期する **場合は** 、Sandboxを確認します。

1. 警告を読み、「資格情報を **確認**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >マッピングを調べて [マッピングをカスタマイズしたい場合](https://docs.marketo.com/display/public/DOCS/Edit+Initial+Field+Mappings)、その機会はこれだけです。 「開始」「Salesforce同期」をクリックすると、同期が完了します。

## 開始Salesforce同期 {#start-salesforce-sync}

1. 「 **開始Salesforce Sync** 」をクリックして、永続的なMarketor-Salesforce同期を開始します。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketorは、Salesforceの同期に対して、またはリードを手動で入力した場合に、自動的に重複除外を行いません。

1. [ **開始同期**]をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >初期同期が完了するまでの時間は、データベースのサイズと複雑さに応じて異なります。

## 同期の検証 {#verify-sync}

Marketorは、管理領域でSalesforce同期のステータスメッセージを提供します。 次の手順に従って、同期が正しく動作していることを確認できます。

1. Marketoで、「 **管理者**」、「 **Salesforce**」の順にクリックします。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同期ステータスは、右上隅に表示されます。 次の3つのメッセージのいずれかが表示されます。 **前回の同期**、 **同期中**、 **失敗**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Marketoの最も強力な機能の1つの設定が完了しました。

>[!NOTE]
>
>**関連記事**
>
>* [手順1/3:Salesforce追加に対するマーケティング担当者のフィールド(Enterprise/Unlimited)](step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順2/3:Marketor向けSalesforceユーザーの作成(Enterprise/Unlimited)](step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [SalesforceAppExchangeへのMarketo Sales Insightパッケージのインストール](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Salesforce Enterprise/UnlimitedでのMarketor Sales Insightの設定](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>* [オプションの手順](http://docs.marketo.com/display/docs/optional+steps)

>



