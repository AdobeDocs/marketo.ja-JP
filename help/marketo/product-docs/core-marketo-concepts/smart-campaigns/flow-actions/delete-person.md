---
unique-page-id: 1147082
description: 人物の削除 - Marketo ドキュメント - 製品ドキュメント
title: 人物の削除
exl-id: 40039444-9b2a-4b80-93bc-7da3d6e9475c
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '113'
ht-degree: 35%

---

# 人物の削除 {#delete-person}

誤ったユーザーがデータベースに取り込まれることもあります。 人物の削除フローステップで削除できます。

![](assets/delete-person-1.png)

>[!CAUTION]
>
>人物を削除すると、その人物の履歴 RCE データもすべて削除されます。これは元に戻せません。

1. フローステップをドラッグすると、CRM からも自動的に削除されるように設定されます。

   ![](assets/delete-person-2.png)

1. 以下のように、を CRM から削除するのではなく、Marketo Engageから削除できます。

   ![](assets/delete-person-3.png)

>[!NOTE]
>
>CRM からの人物の削除 _[!DNL Salesforce]_ でのみ機能します。 Marketoからユーザーを削除し、そのユーザーを [!DNL Salesforce] に保持することを選択した場合、[!DNL Salesforce] レコードが更新されるたびに、そのユーザーはMarketoで再作成されます。
