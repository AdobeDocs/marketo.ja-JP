---
description: Salesforce との配信停止の同期 — Marketoドキュメント — 製品ドキュメント
title: Salesforce との配信停止の同期
hide: true
hidefromtoc: true
exl-id: b5b0f625-e38c-4a03-81e7-010082001636
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 9%

---

# Salesforce との配信停止の同期 {#syncing-unsubscribes-with-salesforce}

## Salesforce との同期を停止する際の要件 {#requirements-for-unsubscribes-to-sync-to-salesforce}

* 配信停止同期を有効にする必要があります（夜間同期）
* Salesforce にオプトアウトフィールドをインストールする必要があります
* Marketo Sales の担当者レコードには Salesforce ID が必要です

**配信停止をプッシュ**

Marketo Sales で配信停止が収集された場合、それをリアルタイムで Salesforce にプッシュし、同期対象として選択したオプトアウトフィールドのいずれかを更新します。 Salesforce 同期を無効にしても、配信停止はメールオプトアウトに引き続きプッシュされます。

**同期を停止**

配信停止同期（以下の手順 3）を有効にすると、夜間の同期が有効になります。 同期は 1 日に 1 回、午後 8:00 PST 頃に実行されます。 MSE/ToutApp 内のすべての配信停止を、Salesforce のオプトアウトフィールドと双方向同期します。

## Salesforce への配信停止同期の設定 {#configure-unsubscribe-sync-to-salesforce}

ユーザーは、Marketoも同期できる標準の電子メールオプトアウトフィールドに登録解除を同期するか、Marketoセールスオプトアウトフィールドに同期して販売登録解除とマーケティング登録解除を区別できるように指定できます。

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-1.png)

1. 「管理設定」で、を選択します。 **配信停止**.

   ![](assets/syncing-unsubscribes-with-salesforce-2.png)

1. 次をクリック： **統合** タブをクリックします。 「 Salesforce に同期」で、夜間同期を有効にします。

   ![](assets/syncing-unsubscribes-with-salesforce-3.png)

1. 同期先のフィールドを選択します。

   ![](assets/syncing-unsubscribes-with-salesforce-4.png)

   | フィールド | 説明 |
   |---|---|
   | **Salesforce オプトアウトフィールドに同期** | デフォルトで選択され、Salesforce オプトアウトフィールドのみが更新されます。 |
   | **Marketo セールスオプトアウトフィールドに同期** | セールスとマーケティングの配信停止を分ける場合は、このオプションを選択して、 [Marketoセールスオプトアウトフィールド。](#msoo) |

## ページレイアウトの「オプトアウト」フィールドのインストール {#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

メールのオプトアウトは、Salesforce からインストールできる Salesforce の標準フィールドです。 インストールするには、Salesforce 管理者である必要があります。

1. に移動します。 [Salesforce.com](https://salesforce.com) にログインし、

   ![](assets/syncing-unsubscribes-with-salesforce-5.png)

1. ユーザー名をクリックし、「 」を選択します。 **設定**.

   ![](assets/syncing-unsubscribes-with-salesforce-6.png)

1. クイック検索ボックスで、[ 連絡先 ] または [ リード ] を検索します。 このシナリオでは、連絡先ページレイアウトのフィールドをインストールしますが、両方の担当者レコード用にをインストールします。

   ![](assets/syncing-unsubscribes-with-salesforce-7.png)

1. 選択 **ページレイアウト**.

   ![](assets/syncing-unsubscribes-with-salesforce-8.png)

1. 選択 **編集** をクリックします。

   ![](assets/syncing-unsubscribes-with-salesforce-9.png)

1. 選択 **フィールド**.

   ![](assets/syncing-unsubscribes-with-salesforce-10.png)

1. 電子メールオプトアウトをページレイアウトにドラッグ&amp;ドロップします。

   ![](assets/syncing-unsubscribes-with-salesforce-11.png)

1. 「**保存**」をクリックします。

   ![](assets/syncing-unsubscribes-with-salesforce-12.png)

## Marketo セールスオプトアウト {#marketo-sales-opt-out}

Marketoの販売オプトアウトフィールドは、Marketoの販売のカスタマイズ機能をインストールしたユーザーが使用できるカスタムフィールドです。

Marketoセールスカスタマイズ機能を Salesforce に正常にインストールすると、「 Marketoセールスオプトアウト」フィールドが使用可能になります。
