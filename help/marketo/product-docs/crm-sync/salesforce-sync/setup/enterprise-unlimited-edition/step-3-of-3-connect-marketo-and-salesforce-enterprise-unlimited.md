---
unique-page-id: 2360366
description: 手順3/3 -MarketoとSalesforceの接続(Enterprise/Unlimited) -Marketoドキュメント — 製品ドキュメント
title: 手順3/3 -MarketoとSalesforceの接続(Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 手順3/3:MarketoとSalesforceを接続(Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、設定したSalesforceインスタンスと同期するようにMarketoを設定します。

>[!PREREQUISITES]
>
>* [手順1/3:Salesforce追加へのMarketoフィールド(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順2/3:Marketo向けSalesforceユーザーの作成(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## 同期ユーザーセキュリティトークンの取得{#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンをお持ちの場合は、準備のために「同期ユーザー資格情報とKDを設定」に直接進みます。

1. Marketo同期ユーザーを使用してSalesforceにログインし、同期ユーザーの名前をクリックして、**マイ設定**&#x200B;をクリックします。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. クイック検索で「reset」と入力し、「**Reset My Security Token**」をクリックします。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 「**セキュリティトークンをリセット**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   セキュリティトークンは電子メールで送信されます。

## 同期ユーザー資格情報の設定{#set-sync-user-credentials}

1. Marketoで、**管理者**&#x200B;に移動し、**CRM**&#x200B;を選択し、**Salesforce.com](https://Salesforce.com)**&#x200B;と同期をクリックします[

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >[**フィールドを同期**]をクリックする前に、Marketoで不要な](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md)フィールドをすべて非表示にしてください。 [[フィールドの同期]をクリックすると、ユーザーに表示されるすべてのフィールドがMarketoに完全に作成され、削除できません。

1. Salesforce設定([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)、[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md))のパート2で作成したSalesforce同期ユーザー資格情報を入力し、「**フィールドを同期**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Salesforce SandboxにMarketoSandboxを同期する場合は、**Sandbox**&#x200B;を確認してください。

1. 警告を読み、「**資格情報を確認**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >[マッピングを調べてカスタマイズ](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)したい場合は、これが唯一の方法です！ 「開始」「Salesforce同期」をクリックすると、同期が完了します。

## Salesforce 同期の開始 {#start-salesforce-sync}

1. 「**開始Salesforce Sync**」をクリックして、永続的なMarketo-Salesforce同期を開始します。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketoは、Salesforce同期に対して、または手動でリードを入力した場合、自動的に重複を排除しません。

1. **開始同期**&#x200B;をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >初期同期が完了するまでの時間は、データベースのサイズと複雑さに応じて異なります。

## 同期の確認{#verify-sync}

Marketoは、管理領域にSalesforce同期のステータスメッセージを表示します。 次の手順に従って、同期が正しく動作していることを確認できます。

1. Marketoで、**管理者**&#x200B;をクリックし、**Salesforce**&#x200B;をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同期ステータスは、右上隅に表示されます。 次の3つのメッセージのいずれかが表示されます。**前回同期**、**同期中**、または&#x200B;**失敗**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Marketoの最も強力な機能の1つの設定が完了しました。

>[!MORELIKETHIS]
>
>* [手順1/3:Salesforce追加へのMarketoフィールド(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順2/3:Marketo向けSalesforceユーザーの作成(Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [SalesforceAppExchangeでのMarketoSales Insightパッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Salesforce EnterpriseでのMarketo販売インサイトの設定/無制限](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

