---
unique-page-id: 4719291
description: デフォルトのリーダーの姓と会社名の設定 - Marketo ドキュメント - 製品ドキュメント
title: デフォルトのリーダーの姓と会社名の設定
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 43%

---

# デフォルトのリーダーの姓と会社名の設定 {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] には、リードおよび連絡先の姓および会社名が必要です（最小限）。 不完全なレコードは [!DNL Salesforce] と同期されません。 部分的なレコードを同期する場合は、[!DNL Salesforce] で使用するMarketoのデフォルト値を設定する必要があります。

1. **[!UICONTROL Admin]** に移動し、「**[!DNL Salesforce]**」をクリックします。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 「**[!UICONTROL 同期オプションを編集]**」をクリックします。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. **[!UICONTROL デフォルトのユーザーの姓]** と **[!UICONTROL デフォルトのユーザーの会社]** を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engageは、レコードが最初にSalesforceに同期され、かつ必須フィールドのいずれかが空の場合にのみ、デフォルト値を割り当てます。

これで完了です。ユーザーに姓や会社名がない場合は常に、Marketo がレコードの同期時にデフォルト値を追加します。
