---
unique-page-id: 14746188
description: Salesforceとの登録解除 —Marketoドキュメント — 製品ドキュメント
title: Salesforceとの登録解除の同期
exl-id: 1694d7bf-d2f6-4950-8a3e-c7d89c37b276
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 5%

---

# Salesforceとの登録解除{#syncing-unsubscribes-with-salesforce}

## Salesforceとの同期を取り消すための要件{#requirements-for-unsubscribes-to-sync-to-salesforce}

* 「登録解除同期」を有効にする必要があります（夜間同期用）
* フィールドオプトアウトをSalesforceにインストールする必要があります
* Sales ConnectのユーザーレコードにはSalesforce IDが必要です

**プッシュ解除**

Sales Connectで登録解除が収集されると、Salesforceにリアルタイムでプッシュして、同期対象として選択したいずれかのオプトアウトフィールドを更新します。 Salesforceの同期を無効にしている場合は、登録解除を電子メールに引き続きプッシュオプトアウトします。

**登録解除同期**

登録解除同期を有効にした場合（下の手順3を参照）、夜間同期が有効になります。 同期は、午後8時(PST)頃に1日1回実行されます。 MSE/ToutApp内のすべての購読解除をSalesforceのフィールドと双方向オプトアウトに同期します。

## Salesforceへの登録解除同期の設定{#configure-unsubscribe-sync-to-salesforce}

ユーザーは、登録解除とMarketoが同期できる標準の電子メールオプトアウトフィールドを同期するか、またはMarketo販売フィールドと同期して、販売登録取り消しとマーケティング登録取り消しを区別できるようにするかを決定できます。

1. [Webアプリケーション](https://toutapp.com/login)に移動し、歯車アイコンをクリックして、**設定**&#x200B;を選択します。

   ![](assets/one-1.png)

1. 「管理設定」で、「**購読解除**」を選択します。

   ![](assets/two-2.png)

1. **Salesforce**&#x200B;と同期をクリックし、夜間同期を有効にします。

   ![](assets/three-2.png)

1. 同期先のフィールドを選択します。

   ![](assets/4.png)

   | フィールド | 詳細 |
   |---|---|
   | **Salesforce オプトアウトフィールドに同期** | デフォルトで選択されている場合は、Salesforceフオプトアウトィールドのみが更新されます。 |
   | **Marketo セールスオプトアウトフィールドに同期** | 販売とマーケティングの登録解除を分割する場合は、このオプションを選択して、[Marketoの販売フィールドをオプトアウト追加更新します。](#msoo) |

## ページレイアウトオプトアウトのフィールドのインストール{#installing-the-opt-out-field-in-the-page-layout}

**メールオプトアウト**

電子メールは、Salesforceからインストールできる、Salesforceの標準フィールドです。 インストールするには、Salesforce管理者である必要があります。

1. [Salesforce.com](https://salesforce.com)に移動し、サインインします。

   ![](assets/five-1.png)

1. ユーザー名をクリックし、「**セットアップ**」を選択します。

   ![](assets/six-1.png)

1. [クイック検索]ボックスで、[連絡先]または[リード]を検索します。 このシナリオでは、[連絡先]ページのレイアウトにフィールドをインストールしますが、両方のユーザーレコードに対してインストールを行います。

   ![](assets/seven-1.png)

1. 「**ページレイアウト**」を選択します。

   ![](assets/eight-1.png)

1. フィールドを追加するページレイアウトの横にある「**編集**」を選択します。

   ![](assets/nine.png)

1. 「**フィールド**」を選択します。

   ![](assets/ten.png)

1. 電子メールをページレイアウトにドラッグ&amp;ドロップオプトアウトします。

   ![](assets/11.png)

1. 「**保存**」をクリックします。

   ![](assets/twelve.png)

## Marketo セールスオプトアウト {#marketo-sales-opt-out}

[Marketoオプトアウトの販売数]フィールドは、Marketoの販売数接続のカスタマイズをインストールしたユーザが使用できるカスタムフィールドです。

[Marketo販売接続のカスタマイズ]をSalesforceに正しくインストールすると、[Marketo販売オプトアウト]フィールドが表示されます。
