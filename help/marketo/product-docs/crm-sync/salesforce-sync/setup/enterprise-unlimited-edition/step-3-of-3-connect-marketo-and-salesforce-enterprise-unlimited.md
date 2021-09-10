---
unique-page-id: 2360366
description: 手順 3／3 — Marketo と Salesforce の接続（Enterprise／Unlimited）— Marketo ドキュメント — 製品ドキュメント
title: 手順 3／3 — Marketo と Salesforce の接続（Enterprise／Unlimited）
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
source-git-commit: 8781c6cf2e64543809fe697e75ae6884969a4e40
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 手順 3／3：Marketo と Salesforce の接続（Enterprise／Unlimited） {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、設定済みの Salesforce インスタンスと同期するように Marketo を設定します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順 2／3：Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンを持っている場合は、直接「同期ユーザー認証情報の設定」に進んで、準備を完了させます。

1. Marketo 同期ユーザーで Salesforce にログインし、同期ユーザーの名前をクリックしてから、**My Settings** をクリックします。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. クイック検索で、&quot;reset&quot; と入力して、**Reset My Security Token** をクリックします。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 「**Reset Security Token**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   セキュリティトークンはメールで送信されます。

## 同期ユーザー認証情報の設定 {#set-sync-user-credentials}

1. Marketo で、「**管理**」に移動し、「**CRM**」を選択して、「**[Salesforce .com](https://www.salesforce.com/jp/) との同期**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >同期ユーザーから Marketo で[不要なフィールドをすべて非表示](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)にした後で、「**同期フィールド**」をクリックするようにしてください。「同期フィールド」をクリックすると、ユーザーが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. Salesforce 設定のパート 2 で作成した Salesforce 同期ユーザーの認証情報（[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) または [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)）を入力して、「**同期フィールド**」をクリックします（Marketo Sandbox を Salesforce Sandbox Sandbox に同期している場合のみ、**Sandbox** をオンにします）。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >「ユーザー名」、「パスワード」、「トークン」フィールドの代わりに「Salesforce にログイン」ボタンが表示される場合、Marketo サブスクリプションで OAuth が有効になっています。[この記事を参照](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md)してください。同期が一連の認証情報を使用し始めるとすぐに、**Salesforce の認証情報またはサブスクリプション**&#x200B;を切り替えられなくなります。基本認証を使用する場合は、カスタマーサクセスマネージャーにお問い合わせください。

1. 警告を読んでから、「**認証情報の確認**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >[マッピングを調べてカスタマイズしたい](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)場合、これが唯一のチャンスです。「Salesforce 同期の開始」をクリックすると、同期されます。

## Salesforce 同期の開始 {#start-salesforce-sync}

1. 「**Salesforce 同期の開始**」をクリックして、Marketo と Salesforce の間の永続的な同期を開始します。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo は、Salesforce の同期や、リードを手動で入力した場合には、自動的に重複排除を行いません。

1. 「**同期の開始**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >最初の同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketo の「管理」領域に、Salesforce 同期に関するステータスメッセージが表示されます。次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketo で、「**管理**」をクリックして、「**Salesforce**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同期ステータスは、右上隅に表示されます。**最終同期**、**同期が進行しています**、**失敗**&#x200B;のいずれかのメッセージが表示されます。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Marketo の最も強力な機能の 1 つの設定が完了しました。

>[!MORELIKETHIS]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順 2／3：Marketo 用の Salesforce ユーザーの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Salesforce AppExchange の Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

