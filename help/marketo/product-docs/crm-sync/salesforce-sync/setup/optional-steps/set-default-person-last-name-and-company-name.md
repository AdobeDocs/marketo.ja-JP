---
unique-page-id: 4719291
description: Salesforce syncのデフォルトのユーザー名と会社名を設定する方法について説明します。 管理オプションと同期オプションを使用して、一部のレコードをデフォルト値と同期します。
title: デフォルトのリーダーの姓と会社名の設定
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 66%

---

# デフォルトのリーダーの姓と会社名の設定 {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] のリードと取引先責任者には最低限で姓と会社名が必要です。 不完全なレコードは [!DNL Salesforce] と同期されません。 部分的なレコードを同期する場合は、Marketo が [!DNL Salesforce] で使用するデフォルト値を設定する必要があります。

1. 「**[!UICONTROL 管理者]**」に移動し、「**[!DNL Salesforce]**」をクリックします。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 「**[!UICONTROL 同期オプションを編集]**」をクリックします。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. 「**[!UICONTROL デフォルト人物の姓]**」および「**[!UICONTROL デフォルト人物の会社]**」を入力してから「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage は、レコードが最初に Salesforce に同期されたときに、必須フィールドのいずれかが空の場合にのみ、デフォルト値を割り当てます。

ユーザーに姓または会社名が見つからない場合は、レコードを同期する際にMarketoがデフォルト値を追加します。
