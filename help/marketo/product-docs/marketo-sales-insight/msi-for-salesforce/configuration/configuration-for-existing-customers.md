---
unique-page-id: 42762519
description: 既存顧客の設定 - Marketo ドキュメント - 製品ドキュメント
title: 既存顧客の設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
source-git-commit: 0701121597f33580ada09fe975c1740cb55f945d
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 100%

---

# 既存顧客の設定 {#configuration-for-existing-customers}

新しいインサイトダッシュボードの使用を開始するには、次の設定を行ってください。

>[!PREREQUISITES]
>
>Salesforce パッケージが最新バージョンにアップグレードされていることを確認してください

## Marketo での Sales Insight の設定 {#configure-sales-insight-in-marketo}

1. ブラウザーで新しいタブを開き、Marketo アカウントから Marketo Sales Insights の資格情報を取得します。

1. 「**管理者**」領域に移動します。

   ![](assets/configuration-for-existing-customers-1.png)

1. 「**Sales Insight**」をクリックします。

   ![](assets/configuration-for-existing-customers-2.png)

1. 「**表示**」を使用して、Rest API 資格情報を設定します。

   ![](assets/configuration-for-existing-customers-3.png)

1. 確認ポップアップが表示されます。「**OK**」をクリックします。

## Salesforce での Sales Insight の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**設定**」をクリックします。

   ![](assets/configuration-for-existing-customers-4.png)

1. 「**リモートサイトの設定**」を検索して選択します。

   ![](assets/configuration-for-existing-customers-5.png)

1. 「**新規リモートサイト**」をクリックします。

   ![](assets/configuration-for-existing-customers-6.png)

1. リモートサイト名（「MarketoRestAPI」など）とリモートサイト URL（Marketo の Rest API 設定パネルの API URL）を入力します。

   ![](assets/configuration-for-existing-customers-7.png)

1. 「**保存**」をクリックします。

   ![](assets/configuration-for-existing-customers-8.png)

   Rest API 用のリモートサイト設定が作成されました。

## Marketo Sales Insight へのアクセス {#access-marketo-sales-insight}

1. Marketo の Sales Insight 管理ページの Rest API パネルから資格情報をコピーします。Salesforce の Sales Insight 設定ページの Rest API セクションに貼り付けます。

1. API 秘密鍵を入力します。

   ![](assets/configuration-for-existing-customers-9.png)
