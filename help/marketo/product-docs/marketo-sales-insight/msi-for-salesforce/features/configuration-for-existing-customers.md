---
unique-page-id: 42762519
description: 既存顧客の設定 — Marketto Docs — 製品ドキュメント
title: 既存のお客様の設定
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---


# 既存のお客様の設定 {#configuration-for-existing-customers}

新しいインサイトダッシュボードの使用を開始するには、次の設定を行ってください。

>[!PREREQUISITES]
>
>Salesforceパッケージを最新バージョンにアップグレードしたことを確認してください

## MarketorでのSales Insightの設定 {#configure-sales-insight-in-marketo}

1. ブラウザーで新しいタブを開き、MarketorアカウントからMarketor Sales Insightsの資格情報を取得します。
1. 「 **管理者** 」領域に移動します。

   ![](assets/configure-1.png)

1. [ **販売インサイト**]をクリックします。

   ![](assets/configure-2.png)

1. 「 **表示** 」をクリックして、Rest API秘密鍵証明書を入力します。

   ![](assets/configure-3.png)

1. 確認ポップアップが表示されます。 「 **OK**」をクリックします。

## SalesforceでのSales Insightの設定 {#configure-sales-insight-in-salesforce}

1. Salesforceで、「 **セットアップ**」をクリックします。

   ![](assets/sfdc-1.png)

1. [ **リモートサイトの設定**]を検索して選択します。

   ![](assets/sfdc-2.png)

1. [ **新規リモートサイト**]をクリックします。

   ![](assets/sfdc-3.png)

1. リモートサイト名（「MarketoRestAPI」など）とリモートサイトURL（MarketoのRest API設定パネルから取得したAPI URL）を入力します。

   ![](assets/sfdc-4.png)

1. 「 **保存**」をクリックします。

   ![](assets/sfdc-5.png)

   Rest APIのリモートサイト設定が作成されました。

## マーケティングに対する販売インサイトへのアクセス {#access-marketo-sales-insight}

1. MarketorのSales Insight管理者ページのRest APIパネルから秘密鍵証明書をコピーします。 それらをSalesforceのSales Insight設定ページのRest APIセクションに貼り付けます。
1. API秘密鍵を入力します。

   ![](assets/config.png)

