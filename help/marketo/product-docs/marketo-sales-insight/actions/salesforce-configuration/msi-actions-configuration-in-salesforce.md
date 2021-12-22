---
description: Salesforce での MSI アクション設定 — Marketo Docs — 製品ドキュメント
title: Salesforce での MSI アクション設定
hide: true
hidefromtoc: true
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: daff9a98605b8a5c89c538f711fecb5b7a382f84
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Salesforce での MSI アクション設定 {#msi-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>のインストールとアップグレード [MSI アクションパッケージ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) を Salesforce インスタンスに追加します。

## CRM 全体で MSI-Actions を有効にする {#enabling-msi-actions-across-the-crm}

1. Salesforce で、 **Marketo Sales Insight 設定** タブをクリックします。

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

   >[!NOTE]
   >
   >上部のバーに「Marketo Sales Insight 設定」が表示されない場合は、 **+** 署名し、「すべてのタブ」の下に表示されます。

1. を選択します。 **MSI アクションを有効にする** チェックボックス。

   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. API 秘密鍵を入力します。

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

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

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. MSI アクションを無効にするには、[ アクション ] 設定で対応する機能をオフにします。

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

>[!NOTE]
>
>ガバナンス設定は、すべての MSI ユーザーに適用できます。
