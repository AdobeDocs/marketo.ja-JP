---
unique-page-id: 4719291
description: デフォルトの個人の姓と会社名の設定 — Marketto Docs — 製品ドキュメント
title: デフォルトの個人の姓と会社名の設定
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# デフォルトの個人の姓と会社名を設定{#set-default-person-last-name-and-company-name}

Salesforceでは、リードと連絡先に姓と会社名が（最小）必要です。 不完全なレコードはSalesforceに同期されません。 部分的なレコードを同期する場合は、Salesforceで使用するMarketoのデフォルト値を設定する必要があります。

1. **管理者**&#x200B;に移動し、**Salesforce**&#x200B;をクリックします。

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. 「**同期オプションを編集**」をクリックします。

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. **デフォルトの個人の姓**&#x200B;と&#x200B;**デフォルトの個人会社**&#x200B;を入力し、**保存**&#x200B;をクリックします。

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >レコードが最初にSalesforceに同期されたとき、および必須フィールドのいずれかが空の場合にのみ、Marketoがデフォルト値を割り当てます。

それだ！ 人に姓や会社名がない場合は常に、レコードの同期時にデフォルト値が追加されます。
