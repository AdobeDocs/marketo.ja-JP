---
description: Salesforce での Sales Insight アクションの設定 — Marketoドキュメント — 製品ドキュメント
title: Salesforce での Sales Insight アクション構成
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: ba1357e6970ba4e3dc496d27272d067ac87c5e6d
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 5%

---

# Salesforce での Sales Insight アクション構成 {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [インストール](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) または [アップグレード](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Salesforce インスタンス内の Sales Insight パッケージ
>* [Salesforce Enterprise／Unlimited での Marketo Sales Insight の設定](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## Salesforce に新しいリモートサイトを追加 {#add-new-remote-site-in-salesforce}

1. Salesforce で、 **設定**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. 「リモートサイト」を検索し、を選択します。 **リモートサイト設定**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. クリック **新規リモートサイト**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. リモートサイト名を入力します（「MarketoSalesInsight」など）。 リモートサイトの URL (https://ims-na1-stg1.adobelogin.com) を入力し、 **保存**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## CRM 全体での Sales Insight アクションの有効化 {#enabling-sales-insight-actions-across-the-crm}

1. Salesforce で、 **Marketo Sales Insight 設定** タブをクリックします。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >上部のバーに「Marketo Sales Insight 設定」が表示されない場合は、 **+** 署名し、「すべてのタブ」の下に表示されます。

1. を選択します。 **MSI アクションを有効にする** チェックボックス。

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. API 秘密鍵を入力します。

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >API 秘密鍵をお持ちでない場合は、 [この記事](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. 終了したら「**保存**」をクリックします。

これにより、機能の概要記事で概要を説明しているすべての MSI アクション機能が自動的に有効になります。

>[!NOTE]
>
>[MSI アクションを有効にする ] チェックボックスをオフにするだけで、すべての MSI アクション機能を無効にすることができます。

## MSI-Actions ガバナンス {#msi-actions-governance}

1. 今後のセクションで、セールスキャンペーンや「タスク」タブを無効にすることができます。 これは、リード、連絡先、アカウント、商談の各パネルに適用されます。

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. MSI アクションを無効にするには、[ アクション ] 設定で対応する機能をオフにします。

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>ガバナンス設定は、すべての MSI ユーザーに適用できます。
