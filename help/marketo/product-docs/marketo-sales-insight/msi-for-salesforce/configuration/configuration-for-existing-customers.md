---
unique-page-id: 42762519
description: 既存顧客の設定 - Marketo ドキュメント - 製品ドキュメント
title: 既存顧客の設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 49%

---

# 既存顧客の設定 {#configuration-for-existing-customers}

新しいインサイトダッシュボードの使用を開始するには、次の設定を行ってください。

>[!PREREQUISITES]
>
>[!DNL Salesforce] パッケージが最新バージョンにアップグレードされていることを確認してください

## Marketoでの [!DNL Sales Insight] の設定 {#configure-sales-insight-in-marketo}

1. ブラウザーで新しいタブを開き、Marketo アカウントから [!DNL Marketo Sales Insights] 資格情報を取得します。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/configuration-for-existing-customers-1.png)

1. 「**[!UICONTROL Sales Insight]**」をクリックします。

   ![](assets/configuration-for-existing-customers-2.png)

1. 「**[!UICONTROL 表示]**」を使用して、Rest API 資格情報を設定します。

   ![](assets/configuration-for-existing-customers-3.png)

1. 確認ポップアップが表示されます。「**[!UICONTROL OK]**」をクリックします。

## [!DNL Sales Insight] での [!DNL Salesforce] の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/configuration-for-existing-customers-4.png)

1. 「**[!UICONTROL リモートサイトの設定]**」を検索して選択します。

   ![](assets/configuration-for-existing-customers-5.png)

1. 「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configuration-for-existing-customers-6.png)

1. [!UICONTROL  リモートサイト名 ] （「MarketoRestAPI」のようなものです）と [!UICONTROL  リモートサイト URL] （Marketoの Rest API 設定パネルからの API URL）を入力します。

   ![](assets/configuration-for-existing-customers-7.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/configuration-for-existing-customers-8.png)

   Rest API 用のリモートサイト設定が作成されました。

## Marketo Sales Insight へのアクセス {#access-marketo-sales-insight}

1. 管理ページの Rest API パネルから資格情報 [!DNL Marketo’s Sales Insight] コピーします。 これらをSalesforceの [!DNL Sales Insight] 設定ページの Rest API セクションに貼り付けます。

1. [!UICONTROL API 秘密鍵 ] を入力します。

   ![](assets/configuration-for-existing-customers-9.png)
