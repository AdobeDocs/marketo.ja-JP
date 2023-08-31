---
description: Salesforce との登録解除の同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce との登録解除の同期
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 100%

---

# Salesforce との登録解除の同期 {#syncing-unsubscribes-with-salesforce}

登録解除を Salesforce の「オプトアウト」フィールドと同期する場合、Salesforce 登録解除の同期を使用できます。

## Salesforce と登録解除を同期する際の要件 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 登録解除の同期を有効にする必要があります（夜間同期）
* Salesforce にオプトアウトフィールドをインストールする必要があります
* Marketo Sales の人物レコードには Salesforce ID が必要です

**登録解除のプッシュ**

Marketo Sales で登録解除が収集された場合、それをリアルタイムで Salesforce にプッシュし、同期対象として選択したオプトアウトフィールドのいずれかを更新します。Salesforce 同期を無効にしても、登録解除はメールオプトアウトに引き続きプッシュされます。

**登録解除の同期**

登録解除を同期を有効にする（以下の手順 3）と、夜間同期が有効になります。同期は 1 日に 1 回、午後 8:00（PST）頃に実行されます。Marketo Sales 内のすべての登録解除と Salesforce の「オプトアウト」フィールドが双方向に同期されます。

>[!NOTE]
>
>Salesforce との登録解除の同期は、登録解除を同期しますが、再登録は同期しません。Marketo Sales および Salesforce から登録解除を削除する場合、Salesforce で登録解除のチェックをオフにして、Marketo Sales で登録解除を削除します。

## Salesforce に登録解除の同期を設定 {#configure-unsubscribe-sync-to-salesforce}

ユーザーは、Marketo も同期できる標準のメールオプトアウトフィールドと登録解除を同期するか、Marketo Sales オプトアウトフィールドに同期して、セールスの登録解除とマーケティングの登録解除を区別できるように指定できます。

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. 「管理者設定」で「**登録解除**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 「**統合**」タブをクリックします。「Salesforce に同期」で、夜間同期を有効にします。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 同期先のフィールドを選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | フィールド | 説明 |
   |---|---|
   | **Salesforce オプトアウトフィールドに同期** | デフォルトで選択され、Salesforce オプトアウトフィールドのみが更新されます。 |
   | **Marketo Sales オプトアウトフィールドに同期** | セールスとマーケティングの登録解除を分ける場合は、このオプションを選択して、追加の [Marketo Sales オプトアウトフィールド](#msoo)を更新します。 |

## ページレイアウトの「オプトアウト」フィールドのインストール {#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

メールのオプトアウトは、Salesforce からインストールできる Salesforce の標準フィールドです。インストールするには、Salesforce 管理者である必要があります。

1. [Salesforce.com](https://salesforce.com) に移動し、ログインします。

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. ユーザー名をクリックし、「**設定**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. クイック検索ボックスで、取引先責任者またはリードを検索します。このシナリオでは、取引先責任者ページレイアウトのフィールドをインストールしますが、両方の人物レコード用にインストールする場合もあります。

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. 「**ページレイアウト**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. フィールドを追加するページレイアウトの横にある「**編集**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. 「**フィールド**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. メールオプトアウトをページレイアウトにドラッグ＆ドロップします。

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. 「**保存**」をクリックします。

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo Sales オプトアウト {#marketo-sales-opt-out}

Marketo Sales オプトアウトフィールドは、[AppExchange から](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"} Marketo Sales Insight パッケージをインストールしたユーザーが使用できるカスタムフィールドです。

Marketo Sales Insight パッケージを AppExchange から Salesforce に正常にインストールすると、「Marketo Sales オプトアウト」フィールドが表示されます。
