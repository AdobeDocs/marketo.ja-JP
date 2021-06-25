---
unique-page-id: 42762519
description: 既存顧客の設定 — Marketoドキュメント — 製品ドキュメント
title: 既存顧客の設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
source-git-commit: 0701121597f33580ada09fe975c1740cb55f945d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 2%

---

# 既存顧客の設定 {#configuration-for-existing-customers}

新しいインサイトダッシュボードの使用を開始するには、次の設定を行ってください。

>[!PREREQUISITES]
>
>Salesforceパッケージが最新バージョンにアップグレードされていることを確認してください。

## Marketoでの販売インサイトの設定 {#configure-sales-insight-in-marketo}

1. ブラウザーで新しいタブを開き、MarketoアカウントからMarketo Sales Insightsの資格情報を取得します。

1. **管理**&#x200B;領域に移動します。

   ![](assets/configuration-for-existing-customers-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/configuration-for-existing-customers-2.png)

1. 「**表示**」をクリックして、Rest APIの資格情報を設定します。

   ![](assets/configuration-for-existing-customers-3.png)

1. 確認のポップアップが表示されます。 「**OK**」をクリックします。

## Salesforceでの販売インサイトの設定 {#configure-sales-insight-in-salesforce}

1. Salesforceで、「**設定**」をクリックします。

   ![](assets/configuration-for-existing-customers-4.png)

1. **リモートサイト設定**&#x200B;を検索して選択します。

   ![](assets/configuration-for-existing-customers-5.png)

1. 「**新しいリモートサイト**」をクリックします。

   ![](assets/configuration-for-existing-customers-6.png)

1. 「リモートサイト名」（「MarketoRestAPI」など）と、「リモートサイトURL」(MarketoのRest API設定パネルのAPI URL)を入力します。

   ![](assets/configuration-for-existing-customers-7.png)

1. 「**保存**」をクリックします。

   ![](assets/configuration-for-existing-customers-8.png)

   これで、Rest API用のリモートサイト設定が作成されました。

## Marketo Sales Insight にアクセス {#access-marketo-sales-insight}

1. MarketoのSales Insight AdminページのRest APIパネルから資格情報をコピーします。 それらを、SalesforceのSales Insight設定ページのRest APIセクションに貼り付けます。

1. API秘密鍵を入力します。

   ![](assets/configuration-for-existing-customers-9.png)
