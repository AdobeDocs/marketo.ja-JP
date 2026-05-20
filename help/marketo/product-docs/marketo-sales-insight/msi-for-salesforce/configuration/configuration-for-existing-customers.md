---
unique-page-id: 42762519
description: 既存のSalesforceのお客様に対してMarketo Sales Insightを設定する方法について説明します。 古いパッケージから更新するか、アクションを追加します。
title: 既存顧客の設定
exl-id: e365f6b5-a3ec-492e-9348-2d3226e6c7eb
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/kdiRnqpm3kJXIPz2QLQS-AF3f04UIPuOS6c836EXlxo
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 90%

---

# 既存顧客の設定 {#configuration-for-existing-customers}

新しいインサイトダッシュボードの使用を開始するには、次の設定を行ってください。

>[!PREREQUISITES]
>
>[!DNL Salesforce] パッケージが最新バージョンにアップグレードされていることを確認してください。

## Marketo での [!DNL Sales Insight] の設定 {#configure-sales-insight-in-marketo}

1. ブラウザーで新しいタブを開き、Marketo アカウントから [!DNL Marketo Sales Insights] の資格情報を取得します。

1. 「**[!UICONTROL 管理者]**」領域に移動します。

   ![](assets/configuration-for-existing-customers-1.png)

1. 「**[!UICONTROL セールスインサイト]**」をクリックします。

   ![](assets/configuration-for-existing-customers-2.png)

1. 「**[!UICONTROL 表示]**」を使用して、Rest API 資格情報を設定します。

   ![](assets/configuration-for-existing-customers-3.png)

1. 確認ポップアップが表示されます。 「**[!UICONTROL OK]**」をクリックします。

## [!DNL Salesforce] での [!DNL Sales Insight] の設定 {#configure-sales-insight-in-salesforce}

1. Salesforce で、「**[!UICONTROL 設定]**」をクリックします。

   ![](assets/configuration-for-existing-customers-4.png)

1. 「**[!UICONTROL リモートサイトの設定]**」を検索して選択します。

   ![](assets/configuration-for-existing-customers-5.png)

1. 「**[!UICONTROL 新規リモートサイト]**」をクリックします。

   ![](assets/configuration-for-existing-customers-6.png)

1. [!UICONTROL リモートサイト名]（「MarketoRestAPI」など）と[!UICONTROL リモートサイト URL]（Marketo の Rest API 設定パネルの API URL）を入力します。

   ![](assets/configuration-for-existing-customers-7.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/configuration-for-existing-customers-8.png)

   Rest API 用のリモートサイト設定が作成されました。

## Marketo セールスインサイトへのアクセス {#access-marketo-sales-insight}

1. [!DNL Marketo’s Sales Insight] 管理ページの Rest API パネルから資格情報をコピーします。 Salesforce の [!DNL Sales Insight] 設定ページの Rest API セクションに貼り付けます。

1. [!UICONTROL API 秘密鍵]を入力します。

   ![](assets/configuration-for-existing-customers-9.png)
