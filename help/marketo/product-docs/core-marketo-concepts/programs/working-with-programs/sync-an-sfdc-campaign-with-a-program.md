---
unique-page-id: 1147154
description: SFDC キャンペーンとプログラムの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC キャンペーンとプログラムの同期
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 9e51ece12742152040dbbcb6a1584fba28e863ff
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 52%

---

# SFDC キャンペーンとプログラムの同期 {#sync-an-sfdc-campaign-with-a-program}

Marketo Engageを使用すると、プログラムをと同期できます [!DNL Salesforce] キャンペーンを使用して、両方のシステムの同じリストの人（ステータスを含む）を維持できます。 それでは始めましょう。

>[!PREREQUISITES]
>
>まず、[ [!DNL Salesforce]  キャンペーンの同期を有効にする](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"}必要があります。

>[!CAUTION]
>
>SFDC キャンペーンをMarketo Engageプログラムと同期する場合、プログラムの子キャンペーンに対して、暗黙の SFDC アクション（SFDC キャンペーンに追加、SFDC に同期など）が無効になります。

1. 「**[!UICONTROL マーケティング活動]**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. プログラムを選択します。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 「**[!UICONTROL プログラムアクション]**」をクリックし、「**[!UICONTROL Salesforce キャンペーン同期]**」を選択します。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. 選択 **[!UICONTROL 新規作成]** または既存の [!DNL Salesforce] キャンペーン。

   >[!TIP]
   >
   >既存の [!DNL Salesforce] キャンペーン、必ず [プログラムのステータスに一致する [!DNL Salesforce] キャンペーンとMarketoプログラム](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"}.

1. 新しいキャンペーンの名前を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 進行状況が Marketo プログラムのステータスと一致していることを確認します。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   これで完了です。Marketo で変更されたプログラムステータスが常に SFDC キャンペーンに同期され、また逆方向にも同期されるようになりました。
