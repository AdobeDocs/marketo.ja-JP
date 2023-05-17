---
description: Salesforce との配信停止の同期 - Marketo ドキュメント - 製品ドキュメント
title: Salesforce との配信停止の同期
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: f174cba33e18812ac08adf177302d997bbe60c4c
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 84%

---

# Salesforce との配信停止の同期 {#syncing-unsubscribes-with-salesforce}

## Salesforce と配信停止を同期する際の要件 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 配信停止の同期を有効にする必要があります（夜間同期）
* Salesforce にオプトアウトフィールドをインストールする必要があります
* Marketo Sales の人物レコードには Salesforce ID が必要です

**配信停止のプッシュ**

Marketo Sales で配信停止が収集された場合、それをリアルタイムで Salesforce にプッシュし、同期対象として選択したオプトアウトフィールドのいずれかを更新します。Salesforce 同期を無効にしても、配信停止はメールオプトアウトに引き続きプッシュされます。

**配信停止の同期**

配信停止を同期（以下の手順 3）を有効にすると、夜間の同期が有効になります。同期は 1 日に 1 回、午後 8:00（PST）頃に実行されます。Marketo Sales のすべての配信停止が、Salesforce のオプトアウトフィールドと双方向に同期されます。

## Salesforce に配信停止の同期を設定 {#configure-unsubscribe-sync-to-salesforce}

ユーザは、Marketo も同期できる標準のメールオプトアウトフィールドと配信停止を同期するか、Marketo Sales オプトアウトフィールドに同期して、セールスの配信停止とマーケティングの配信停止を区別できるように指定できます。

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. 「管理者設定」で「**配信停止**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 「**統合**」タブをクリックします。「Salesforce に同期」で、夜間同期を有効にします。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 同期先のフィールドを選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | フィールド | 説明 |
   |---|---|
   | **Salesforce オプトアウトフィールドに同期** | デフォルトで選択され、Salesforce オプトアウトフィールドのみが更新されます。 |
   | **Marketo Sales オプトアウトフィールドに同期** | セールスとマーケティングの配信停止を分ける場合は、このオプションを選択して、追加の [Marketo Sales オプトアウトフィールド](#msoo)を更新します。 |

## ページレイアウトの「オプトアウト」フィールドのインストール {#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

メールのオプトアウトは、Salesforce からインストールできる Salesforce の標準フィールドです。インストールするには、Salesforce 管理者である必要があります。

1. [Salesforce.com](https://salesforce.com) に移動し、ログインします。

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. ユーザ名をクリックし、「**設定**」を選択します。

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

Marketo Sales Opt Out フィールドは、Marketo Sales Insight パッケージをインストールしたユーザーが使用できるカスタムフィールドです [AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

Marketo Sales Insight パッケージをAppExchangeから Salesforce に正常にインストールすると、「 Marketo Sales Opt Out 」フィールドが表示されます。
