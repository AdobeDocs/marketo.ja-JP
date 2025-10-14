---
unique-page-id: 1147154
description: SFDC キャンペーンとプログラムの同期 - Marketo ドキュメント - 製品ドキュメント
title: SFDC キャンペーンとプログラムの同期
exl-id: b95be580-c960-4a76-9d43-c7f624f43d03
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 47%

---

# SFDC キャンペーンとプログラムの同期 {#sync-an-sfdc-campaign-with-a-program}

Marketo Engageを使用すると、プログラムを [!DNL Salesforce] キャンペーンと同期して、両方のシステムで同じ人物のリスト（ステータスを含む）を維持できます。 それでは始めましょう。

>[!PREREQUISITES]
>
>最初に [&#x200B; 有効にする  [!DNL Salesforce]  キャンペーン同期 &#x200B;](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md){target="_blank"} が必要です。

>[!CAUTION]
>
>SFDC キャンペーンをMarketo Engage プログラムと同期する場合、暗黙のSFDC アクション（SFDC キャンペーンに追加、SFDCに同期など）は、プログラムの子キャンペーンに対して無効になります。

1. 「**[!UICONTROL マーケティング活動]**」に移動します。

   ![](assets/login-marketing-activities-1.png)

1. プログラムを選択します。

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. 「**[!UICONTROL プログラムアクション]**」をクリックし、「**[!UICONTROL Salesforce キャンペーン同期]**」を選択します。

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. **[!UICONTROL 新規作成]** を選択するか、既存の [!DNL Salesforce] キャンペーンを選択します。

   >[!TIP]
   >
   >既存の [!DNL Salesforce] キャンペーンを選択する場合は、[&#x200B; キャンペーンのプログラムステータスとMarketo プログラムを一致させる  [!DNL Salesforce]  ことを確認 &#x200B;](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md){target="_blank"} ます。

1. 新しいキャンペーンの名前を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. 進行状況が Marketo プログラムのステータスと一致していることを確認します。

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   これで完了です。Marketo で変更されたプログラムステータスが常に SFDC キャンペーンに同期され、また逆方向にも同期されるようになりました。
