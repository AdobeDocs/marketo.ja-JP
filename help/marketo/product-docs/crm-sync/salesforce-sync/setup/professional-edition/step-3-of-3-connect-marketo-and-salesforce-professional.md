---
unique-page-id: 3571800
description: 手順 3／3 — Marketo と Salesforce の接続（Professional）- Marketo ドキュメント - 製品ドキュメント
title: 手順 3／3 — Marketo と Salesforce の接続（Professional）
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 67%

---

# 手順 3/3:Marketoと [!DNL Salesforce] を接続する（Professional） {#step-of-connect-marketo-and-salesforce-professional}

この記事では、設定済みのSalesforce インスタンスと同期するようにMarketo Engageを設定します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの Salesforce への追加（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [手順 2 / 3：Marketo 用の Salesforce ユーザーの作成（Professional）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンを持っている場合は、直接「同期ユーザー資格情報の設定」に進んで、準備を完了させます。

1. Marketo Sync User を使用してSalesforceにログインし、同期ユーザーの名前をクリックして、**[!UICONTROL My Settings]** をクリックします。

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. ナビゲーションの検索バーに「リセット」と入力し、**[!UICONTROL セキュリティトークンをリセット]** をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. 「**[!UICONTROL Reset Security Token]**」をクリックします。

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   セキュリティトークンはメールで送信されます。

## 同期ユーザー資格情報の設定 {#set-sync-user-credentials}

1. Marketoで、**[!UICONTROL 管理者]** に移動して **[!UICONTROL CRM]** を選択し、**[!UICONTROL Salesforce.com と同期]** をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >同期ユーザーから Marketo で[不要なフィールドをすべて非表示](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"}にした後で、「**[!UICONTROL 同期フィールド]**」をクリックするようにしてください。「同期フィールド」をクリックすると、ユーザーが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. Salesforce設定のパート 2 （[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)、[Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)）で作成したSalesforce Sync ユーザーの資格情報を入力し、「**[!UICONTROL フィールドを同期]**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Marketo Sandbox を Salesforce Sandbox に同期する場合、「**[!UICONTROL サンドボックス]**」のチェックをオンにします。

1. 警告を読んでから、「**[!UICONTROL 資格情報の確認]**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >[マッピングを調べてカスタマイズしたい](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}場合、これが唯一のチャンスです。「Salesforce 同期の開始」をクリックすると、同期されます。

## 同期 [!DNL Salesforce] 開始 {#start-salesforce-sync}

1. 「**[!UICONTROL Salesforce 同期の開始]**」をクリックして、Marketo と Salesforce の間の永続的な同期を開始します。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketoは、[!DNL Salesforce] 同期に対する重複除外、またはリードを手動で追加しても自動的に重複除外を実行しません。

1. 「**[!UICONTROL 同期の開始]**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >最初の同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketoの管理領域に、[!DNL Salesforce] 同期のステータスメッセージが表示されます。 次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketo で、「**[!UICONTROL 管理]**」をクリックして、「**Salesforce**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同期ステータスは、右上隅に表示されます。**[!UICONTROL 最終同期]**、**[!UICONTROL 同期が進行しています]**、**[!UICONTROL 失敗]**&#x200B;のいずれかのメッセージが表示されます。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Marketoの最も強力な機能の 1 つの設定が完了しました。

>[!MORELIKETHIS]
>
>* [Salesforce AppExchange での Marketo Sales Insight パッケージのインストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Salesforce Professional Edition での Marketo Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
