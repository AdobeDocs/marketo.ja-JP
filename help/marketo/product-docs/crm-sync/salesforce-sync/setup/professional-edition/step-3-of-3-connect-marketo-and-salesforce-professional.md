---
unique-page-id: 3571800
description: 手順 3／3 — Marketo と Salesforce の接続（Professional）- Marketo ドキュメント - 製品ドキュメント
title: 手順 3／3 — Marketo と Salesforce の接続（Professional）
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
source-git-commit: 8162db802cae125b406c463fde50d4ffdf0eb621
workflow-type: ht
source-wordcount: '382'
ht-degree: 100%

---

# 手順 3／3：Marketo と Salesforce の接続（Professional） {#step-of-connect-marketo-and-salesforce-professional}

この記事では、設定済みの Salesforce インスタンスと同期するように Marketo を設定します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [手順 2 / 3：Marketo 用の Salesforce ユーザーの作成（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)


## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンを持っている場合は、直接「同期ユーザー認証情報の設定」に進んで、準備を完了させます。

1. Marketo 同期ユーザーで Salesforce にログインし、同期ユーザーの名前をクリックしてから、**My Settings** をクリックします。

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. ナビゲーション検索バーで、「リセット」と入力して、「**セキュリティトークンのリセット**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 「**Reset Security Token**」をクリックします。

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   セキュリティトークンはメールで送信されます。

## 同期ユーザー認証情報の設定 {#set-sync-user-credentials}

1. Marketo で、「**管理**」に移動し、「**CRM**」を選択して、「**[Salesforce .com](https://Salesforce.com) との同期**」をクリックします。。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >同期ユーザーから Marketo で[不要なフィールドをすべて非表示](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)にした後で、「**同期フィールド**」をクリックするようにしてください。「同期フィールド」をクリックすると、ユーザーが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. Salesforce 設定のパート 2 で作成した Salesforce 同期ユーザーの認証情報（[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) または [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)）を入力して、「**同期フィールド**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marketo Sandbox を Salesforce Sandbox に同期する場合、「**サンドボックス**」のチェックをオンにします。

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
>* [Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Salesforce Professional Edition での Marketo Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

