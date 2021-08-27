---
unique-page-id: 2360366
description: 手順3 / 3 -MarketoとSalesforceの接続（Enterprise/無制限） - Marketoドキュメント — 製品ドキュメント
title: 手順3 / 3 -MarketoとSalesforceの接続（エンタープライズ/無制限）
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# 手順3/3:MarketoとSalesforceの接続（Enterprise/無制限） {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、Marketoを設定済みのSalesforceインスタンスと同期するように設定します。

>[!PREREQUISITES]
>
>* [手順1/3:SalesforceへのMarketoフィールドの追加（エンタープライズ/無制限）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順2 / 3:Marketo向けSalesforceユーザーの作成（エンタープライズ/無制限）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンを持っている場合は、Set Sync User Credentials and Kudosに直接進んで準備します。

1. Marketo Sync UserでSalesforceにログインし、同期ユーザーの名前をクリックしてから、**My Settings**&#x200B;をクリックします。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. クイック検索で、&quot;reset&quot;と入力し、**Reset My Security Token**&#x200B;をクリックします。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 「**セキュリティトークンをリセット**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   セキュリティトークンは電子メールで送信されます。

## ユーザーの資格情報の同期の設定 {#set-sync-user-credentials}

1. Marketoで、「**管理**」に移動し、「**CRM**」を選択して、「**[Salesforce.com](https://Salesforce.com)**&#x200B;と同期」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >**「フィールドを同期**」をクリックする前に、Marketoで不要な](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)フィールドをすべて同期ユーザーから非表示にしてください。 [「フィールドを同期」をクリックすると、ユーザーに表示されるすべてのフィールドがMarketoに完全に作成され、削除できなくなります。

1. Salesforce設定のパート2で作成したSalesforce Syncユーザーの資格情報（[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)または[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)）を入力し、「**Sync Fields**」(Marketo Salesforce SandboxをSandboxに同期する場合のみ&#x200B;**をオンにします)をクリックします。**

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >「ユーザー名」、「パスワード」、「トークン」の代わりに「Salesforceへのログイン」ボタンが表示された場合、MarketoサブスクリプションでOAuthが有効になっています。 [この記事](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md)を参照してください。 同期が一連の資格情報を使用し始めるとすぐに、**Salesforceの資格情報またはサブスクリプション**&#x200B;を切り替えることはできません。 基本認証を使用する場合は、カスタマーサクセスマネージャーにお問い合わせください。

1. 警告を読み、「**資格情報を確認**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >[マッピングを調べてカスタマイズしたい場合は](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)、これが唯一のチャンスです。 「Salesforce同期を開始」をクリックすると、完了です。

## Salesforce 同期の開始 {#start-salesforce-sync}

1. 「**Salesforce同期を開始**」をクリックして、永続的なMarketo-Salesforce同期を開始します。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketoは、Salesforceの同期や、リードを手動で入力した場合、自動的に重複排除をおこないません。

1. 「**同期を開始**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >初期同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketoの「管理」領域に、Salesforce同期のステータスメッセージが表示されます。 次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketoで、「**管理者**」をクリックし、「**Salesforce**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同期ステータスは右上隅に表示されます。 次の3つのメッセージのいずれかが表示されます。**最後に同期された**、**処理中の同期**、または&#x200B;**失敗**。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Marketoの最も強力な機能の1つの設定が完了しました。

>[!MORELIKETHIS]
>
>* [手順1/3:SalesforceへのMarketoフィールドの追加（エンタープライズ/無制限）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順2 / 3:Marketo向けSalesforceユーザーの作成（エンタープライズ/無制限）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Marketo Sales InsightパッケージのSalesforceAppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Salesforce Enterprise/無制限でのMarketo Sales Insightの設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

