---
unique-page-id: 42762519
description: 既存顧客の設定 —Marketoドキュメント — 製品ドキュメント
title: 既存のお客様の設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 2%

---

# 既存のお客様の構成{#configuration-for-existing-customers}

新しいインサイトダッシュボードの使用を開始するには、次の設定を行ってください。

>[!PREREQUISITES]
>
>Salesforceパッケージを最新バージョンにアップグレードしたことを確認してください

## MarketoでのSales Insightの設定{#configure-sales-insight-in-marketo}

1. ブラウザーで新しいタブを開き、MarketoアカウントからMarketoのSales Insights資格情報を取得します。

1. **管理者**&#x200B;領域に移動します。

   ![](assets/configure-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/configure-2.png)

1. **表示**&#x200B;をクリックして、Rest APIの秘密鍵証明書を入力します。

   ![](assets/configure-3.png)

1. 確認ポップアップが表示されます。 「**OK**」をクリックします。

## SalesforceでのSales Insightの設定{#configure-sales-insight-in-salesforce}

1. Salesforceで、**セットアップ**&#x200B;をクリックします。

   ![](assets/sfdc-1.png)

1. **リモートサイト設定**&#x200B;を検索して選択します。

   ![](assets/sfdc-2.png)

1. [**新しいリモートサイト**]をクリックします。

   ![](assets/sfdc-3.png)

1. リモートサイト名（「MarketoRestAPI」など）とリモートサイトURL(MarketoのRest API設定パネルのAPI URL)を入力します。

   ![](assets/sfdc-4.png)

1. 「**保存**」をクリックします。

   ![](assets/sfdc-5.png)

   Rest APIのリモートサイト設定が作成されました。

## Marketo Sales Insight にアクセス {#access-marketo-sales-insight}

1. MarketoのSales Insight管理ページのRest APIパネルから秘密鍵証明書をコピーします。 それらをSalesforceのSales Insight設定ページのRest APIセクションに貼り付けます。

1. API秘密鍵を入力します。

   ![](assets/config.png)
