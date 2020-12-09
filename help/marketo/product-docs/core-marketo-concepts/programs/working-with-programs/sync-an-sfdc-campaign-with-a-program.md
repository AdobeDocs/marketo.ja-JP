---
unique-page-id: 1147154
description: SFDCキャンペーンとプログラムの同期 — Marketto Docs — 製品ドキュメント
title: SFDCキャンペーンとプログラムの同期
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# SFDCキャンペーンとプログラムの同期 {#sync-an-sfdc-campaign-with-a-program}

Marketorでは、プログラムをSalesforceキャンペーンと同期して、ステータスを含む両方のシステムで同じリストを維持できます。 始めよう！

>[!PREREQUISITES]
>
>まず、Salesforceキャンペーン同期を [有効にする必要があります](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) 。

>[!CAUTION]
>
>SFDCキャンペーンをMarketoプログラムと同期する場合、プログラムの子キャンペーンに対しては、黙示的なSFDCの操作(SFDCキャンペーンに追加、SFDCに同期など)が無効になります。

1. 「 **マーケティングアクティビティ**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. プログラムを選択します。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 「 **プログラムアクション**」をクリックし、「 **Salesforceキャンペーン同期**」を選択します。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 「**新規作成**」を選択するか、既存のSalesforceキャンペーンを選択します。

   >[!TIP]
   >
   >既存のSalesforceキャンペーンを選択する場合は、SalesforceキャンペーンとMarketoプログラムのプログラムステータスが [一致していることを確認します](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)。

1. 新しいキャンペーンの名前を入力し、「 **保存**」をクリックします。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. これで、キャンペーンの同期の詳細をプログラムの概要ページで確認できます。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   素晴らしい！ 現在は、Marketoのプログラムステータスの変更はすべてSFDCキャンペーンと同期され、その逆も同期されます。

