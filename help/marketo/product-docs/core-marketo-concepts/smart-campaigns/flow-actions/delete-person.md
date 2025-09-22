---
unique-page-id: 1147082
description: 人物の削除 - Marketo ドキュメント - 製品ドキュメント
title: 人物の削除
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 100%

---

# 人物の削除 {#delete-person}

誤った人物がデータベースに格納されることがあります。人物を削除フローステップで削除できます。

![](assets/delete-person-1.png)

>[!CAUTION]
>
>人物を削除すると、その人物の履歴 RCE データもすべて削除されます。これは元に戻せません。

1. フローステップにドラッグすると、CRM からも自動的に削除されるように設定されます。

   ![](assets/delete-person-2.png)

1. 次のように、CRM ではなく Marketo Engage から削除できます。

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>CRM からの人物の削除は、_[!DNL Salesforce]_ でのみ機能します。人物を Marketo から削除し、[!DNL Salesforce] で保持することにした場合、[!DNL Salesforce] のレコードが更新された場合は、Marketo で再作成されます。
