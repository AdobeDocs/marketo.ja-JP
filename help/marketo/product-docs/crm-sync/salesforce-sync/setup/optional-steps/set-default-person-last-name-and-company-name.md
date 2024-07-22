---
unique-page-id: 4719291
description: デフォルトのリーダーの姓と会社名の設定 - Marketo ドキュメント - 製品ドキュメント
title: デフォルトのリーダーの姓と会社名の設定
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 69%

---

# デフォルトのリーダーの姓と会社名の設定 {#set-default-person-last-name-and-company-name}

Salesforce のリードと連絡先には最低限で姓と会社名が必要です。不完全なレコードは Salesforce と同期されません。部分的なレコードを同期する場合は、Marketo が Salesforce で使用するデフォルト値を設定する必要があります。

1. **[!UICONTROL Admin]** に移動し、「**[!DNL Salesforce]**」をクリックします。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 「**[!UICONTROL 同期オプションを編集]**」をクリックします。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. **[!UICONTROL デフォルトのユーザーの姓]** と **[!UICONTROL デフォルトのユーザーの会社]** を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engageは、レコードが最初に Salesforce に同期され、かつ必須フィールドのいずれかが空の場合にのみ、デフォルト値を割り当てます。

これで完了です。ユーザーに姓や会社名がない場合は常に、Marketo がレコードの同期時にデフォルト値を追加します。
