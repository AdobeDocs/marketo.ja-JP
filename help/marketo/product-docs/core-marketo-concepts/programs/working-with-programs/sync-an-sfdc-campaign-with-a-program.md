---
unique-page-id: 1147154
description: SFDCキャンペーンとプログラムの同期 —Marketoドキュメント — 製品ドキュメント
title: SFDCキャンペーンとプログラムの同期
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 1%

---

# SFDCキャンペーンとプログラム{#sync-an-sfdc-campaign-with-a-program}を同期する

Marketoでは、プログラムをSalesforceキャンペーンと同期して、ステータスを含む両方のシステムで同じリストを維持できます。 さあ始めましょう！ 

>[!PREREQUISITES]
>
>最初にSalesforceキャンペーン同期](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md)を[有効にする必要があります。

>[!CAUTION]
>
>SFDCキャンペーンをMarketoプログラムと同期する場合、黙示的なSFDCの操作(SFDCキャンペーンに追加、SFDCに同期など)は、プログラムの子キャンペーンに対して無効になります。

1. **マーケティングアクティビティ**&#x200B;に移動します。

   ![](assets/login-marketing-activities-1.png)

1. プログラムを選択します。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 「**プログラムアクション**」をクリックし、「**Salesforceキャンペーン同期**」を選択します。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 「**新規作成**」を選択するか、既存のSalesforceキャンペーンを選択します。

   >[!TIP]
   >
   >既存のSalesforceキャンペーンを選択する場合は、[がSalesforceキャンペーンとMarketoプログラム](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)のプログラムステータスと一致していることを確認してください。

1. 新しいキャンペーンの名前を入力し、「**保存**」をクリックします。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. これで、キャンペーンの同期の詳細をプログラムの概要ページで確認できます。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   素晴らしい！ 現在は、Marketoでのプログラムステータスの変更はすべてSFDCキャンペーンと同期され、その逆も同期されます。
