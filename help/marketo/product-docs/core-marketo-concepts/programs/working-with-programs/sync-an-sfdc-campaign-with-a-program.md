---
unique-page-id: 1147154
description: Salesforce キャンペーンをMarketo プログラムと同期する方法について説明します。 SFDCとMarketo間でメンバーステータスを同期します。
title: SFDC キャンペーンとプログラムの同期
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: d5258342dd89a8f46a9897e9c7ee8dad4a33df59
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 30%

---

# SFDC キャンペーンとプログラムの同期 {#sync-an-sfdc-campaign-with-a-program}

Marketo Engageを使用すると、プログラムを[!DNL Salesforce]件のキャンペーンと同期して、ステータスを含め、両方のシステムで同じユーザーのリストを維持できます。 それでは始めましょう。

>[!PREREQUISITES]
>
>最初に[&#x200B; キャンペーン同期 [!DNL Salesforce] を有効にする](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}必要があります。

>[!CAUTION]
>
>SFDC キャンペーンとMarketo Engage プログラムを同期する場合、暗黙的なSFDC アクション（例：SFDC キャンペーンへの追加、SFDCへの同期）は、プログラムの子キャンペーンに対して無効になります。

1. **[!UICONTROL マーケティングアクティビティ]**&#x200B;に移動します。

   ![](assets/login-marketing-activities-1.png)

1. プログラムを選択します。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 「**[!UICONTROL プログラムアクション]**」をクリックし、「**[!UICONTROL Salesforce キャンペーン同期]**」を選択します。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. **[!UICONTROL 新規作成]**&#x200B;を選択するか、既存の[!DNL Salesforce] キャンペーンを選択します。

   >[!TIP]
   >
   >既存の[!DNL Salesforce] キャンペーンを選択する場合は、[&#x200B; キャンペーンとMarketo プログラムのプログラムステータスが [!DNL Salesforce] と一致していることを確認してください](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}。

1. 新しいキャンペーンの名前を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 進行状況が Marketo プログラムのステータスと一致していることを確認します。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Marketoのプログラムステータスの変更は、SFDC キャンペーンに同期され、その逆も同様です。
