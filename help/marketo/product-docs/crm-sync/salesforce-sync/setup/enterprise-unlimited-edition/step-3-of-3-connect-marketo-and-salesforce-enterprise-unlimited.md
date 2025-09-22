---
unique-page-id: 2360366
description: 手順 3 / 3 - Marketo と Salesforce の接続（Enterprise／Unlimited）- Marketo ドキュメント - 製品ドキュメント
title: 手順 3 / 3 - Marketo と Salesforce の接続（Enterprise／Unlimited）
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 100%

---

# 手順 3 / 3：Marketo と [!DNL Salesforce] の接続（Enterprise／Unlimited） {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

この記事では、設定済みの [!DNL Salesforce] インスタンスと同期するように Marketo を設定します。

>[!PREREQUISITES]
>
>* [手順 1／3：Marketo フィールドの  [!DNL Salesforce]  への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順 2 / 3：Marketo 用の  [!DNL Salesforce]  ユーザの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## 同期ユーザーセキュリティトークンの取得 {#retrieve-sync-user-security-token}

>[!TIP]
>
>既にセキュリティトークンを持っている場合は、直接「同期ユーザー資格情報の設定」に進んで、準備を完了させます。

1. Marketo 同期ユーザで [!DNL Salesforce] にログインし、同期ユーザの名前をクリックしてから、「**[!UICONTROL マイ設定]**」をクリックします。

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. クイック検索で、&quot;reset&quot; と入力して、**[!UICONTROL Reset My Security Token]** をクリックします。

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. 「**[!UICONTROL Reset Security Token]**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   セキュリティトークンはメールで送信されます。

## 同期ユーザー資格情報の設定 {#set-sync-user-credentials}

1. Marketo で、「**[!UICONTROL 管理]**」に移動し、「**CRM**」を選択して、「**[!UICONTROL Salesforce.com との同期]**」をクリックします。

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >同期ユーザから Marketo で[不要なフィールドをすべて非表示](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md)にした後で、「**[!UICONTROL フィールドを同期]**」をクリックするようにしてください。「[!UICONTROL フィールドを同期]」をクリックすると、ユーザが表示できるすべてのフィールドが Marketo に作成され、削除できなくなります。

1. [!DNL Salesforce] 設定のパート 2 で作成した [!DNL Salesforce] 同期ユーザの資格情報（[Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) または [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)）を入力して、「**[!UICONTROL フィールドを同期]**」をクリックします（Marketo サンドボックスを [!DNL Salesforce] サンドボックスに同期している場合のみ、**[!UICONTROL サンドボックス]**&#x200B;をオンにします）。

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >「ユーザ名」、「パスワード」、「トークン」の各フィールドではなく「[!DNL Salesforce] にログイン」ボタンが表示される場合、Marketo サブスクリプションで OAuth が有効になっています。詳しくは、[この記事を参照](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md)してください。同期が一連の資格情報を使用し始めるとすぐに、**[!DNL Salesforce] の資格情報またはサブスクリプションを切り替えられなくなります**。基本認証を使用する場合は、カスタマーサクセスマネージャーにお問い合わせください。

1. 警告を読んでから、「**[!UICONTROL 資格情報の確認]**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >[マッピングを調べてカスタマイズしたい](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md)場合、これが唯一のチャンスです。「[!UICONTROL Salesforce 同期を開始]」をクリックすると、同期されます。

## [!DNL Salesforce] 同期の開始 {#start-salesforce-sync}

1. 「**[!UICONTROL Salesforce 同期を開始]**」をクリックして、Marketo と [!DNL Salesforce] の間の永続的な同期を開始します。

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo は、[!DNL Salesforce] の同期や、リードを手動で入力した場合には、自動的に重複排除を行いません。

1. 「**[!UICONTROL 同期の開始]**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >最初の同期が完了するまでの時間は、データベースのサイズと複雑さによって異なります。

## 同期の検証 {#verify-sync}

Marketo の「管理」領域に、[!DNL Salesforce] 同期に関するステータスメッセージが表示されます。次の手順に従うことで、同期が正しく機能していることを確認できます。

1. Marketo で、「**[!UICONTROL 管理]**」をクリックして、「**[!UICONTROL Salesforce]**」をクリックします。

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. 同期ステータスは、右上隅に表示されます。**[!UICONTROL 最終同期]**、**[!UICONTROL 同期が進行しています]**、**[!UICONTROL 失敗]**&#x200B;のいずれかのメッセージが表示されます。

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Marketo の最も強力な機能の 1 つの設定が完了しました。

>[!MORELIKETHIS]
>
>* [手順 1 / 3：Marketo フィールドの  [!DNL Salesforce]  への追加（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [手順 2 / 3：Marketo の  [!DNL Salesforce]  ユーザの作成（Enterprise／Unlimited）](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [ [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) での Marketo セールスインサイトパッケージのインストール
>* [ [!DNL Salesforce]  Enterprise／Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) での Marketo セールスインサイトの設定
