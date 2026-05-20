---
unique-page-id: 1147017
description: フローステップでSalesforce タスクを作成する方法を説明します。 誰かがフローに入ったときに、リードオーナーのタスクを作成します。
title: タスクの作成
exl-id: c484d913-1fd8-4716-8caa-0bf318218ca1
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/RJ5nZrVvURtgXEWWZwL2xXzlYOhWjKGSbX-MFTWCwzg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 130
ht-degree: 82%

---

# タスクの作成 {#create-task}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。 タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

![](assets/create-task-1.png)

>[!NOTE]
>
>Marketo 同期ユーザーがタスクを作成する場合、Salesforce でタスクを作成するには「**[!UICONTROL 期限]**」が必須フィールドです。 この値がない場合、Marketo でデフォルトの 5 日が自動入力されます。

デフォルトでは、フローステップは次のようになります。

![](assets/create-task-2.png)

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/create-task-3.png)

>[!TIP]
>
>**[!UICONTROL 件名]**&#x200B;と&#x200B;**[!UICONTROL 説明]**&#x200B;で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。 詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}を参照してください。
