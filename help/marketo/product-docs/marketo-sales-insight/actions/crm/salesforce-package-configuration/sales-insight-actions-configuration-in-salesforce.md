---
description: SalesforceでSales Insight アクションを設定する方法について説明します。 リモートサイトを追加し、MSI アクションを有効にして、API シークレットキーを入力します。
title: Salesforce でのセールスインサイトアクション設定
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
TQID: https://experienceleague.adobe.com/5S-pqmvARTyOj8ED-PrL5zLHGbsBAej8TYuYZw7rtSQ
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 251
ht-degree: 92%

---

# [!DNL Salesforce] での [!DNL Sales Insight Actions] 設定 {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [!DNL Salesforce] インスタンスでのセールスインサイトパッケージの[インストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)または[アップグレード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md)
>* [&#x200B; [!DNL Salesforce]  Enterprise／Unlimited での Marketo セールスインサイトの設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## [!DNL Salesforce] に新しいリモートサイトを追加 {#add-new-remote-site-in-salesforce}

1. [!DNL Salesforce] で、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 「[!UICONTROL リモートサイト]」を検索し、「**[!UICONTROL リモートサイト設定]**」を選択します。
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. 「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. リモートサイト名を入力します（「MarketoSalesInsight1」など）。 リモートサイトの URL `https://ims-na1.adobelogin.com` を入力し、「**[!UICONTROL 保存」をクリックします。]**

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. もう一度「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. リモートサイト名を入力します（「MarketoSalesInsight2」など）。 リモートサイトの URL `https://mkto-sales-connect.adobe.io` を入力し、「**[!UICONTROL 保存]**」をクリックします。

## CRM 全体で [!DNL Sales Insight Actions] を有効にする {#enabling-sales-insight-actions-across-the-crm}

1. [!DNL Salesforce] で、「**[!UICONTROL Marketo セールスインサイト設定]**」タブをクリックします。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >上部のバーに「[!UICONTROL Marketo セールスインサイト設定]」が表示されない場合は、「**+**」記号をクリックし、「すべてのタブ」から見つけます。

1. 「**[!UICONTROL MSI アクションを有効にする]**」チェックボックスをオンにします。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. [!UICONTROL API 秘密鍵]を入力します。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >[!UICONTROL API 秘密鍵]をお持ちでない場合は、[この記事](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)の手順を参照してください。

1. 終了したら「**[!UICONTROL 保存]**」をクリックします。

これにより、機能の概要記事で概要を説明しているすべての MSI アクション機能が自動的に有効になります。

>[!NOTE]
>
>「MSI アクションを有効にする」チェックボックスをオフにするだけで、すべての MSI アクション機能を無効にすることができます。

## MSI アクションのガバナンス {#msi-actions-governance}

1. 今後提供されるセクションで、セールスキャンペーンや「タスク」タブを無効にすることができます。 これは、リード、取引先責任者、アカウント、商談の各パネルに適用されます。

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. MSI アクションを無効にするには、「[!UICONTROL アクション設定]」で対応する機能のチェックを外します。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>ガバナンス設定は、すべての MSI ユーザに適用できます。
