---
unique-page-id: 37356429
description: フローステップからMicrosoft Dynamicsでタスクを作成する方法を説明します。 誰かがフローに入ったときに、所有者のタスクを作成します。
title: Microsoft でのタスクの作成
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/qQL3O4Vi8ncdlXtk2gvraWzquz3oZx5B-1YWTkwdVac
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 86%

---

# Microsoft でのタスクの作成 {#create-task-in-microsoft}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。 タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

「Microsoft でタスクを作成」は、[!DNL Microsoft] で人物（リードまたは取引先責任者）に関連するアクティビティの下にタスクを作成します。

>[!NOTE]
>
>このフローステップは、スマートキャンペーンで、フィルターではなく、_トリガーで使用された場合にのみ機能_&#x200B;します。

デフォルトでは、フローステップは次のようになります。

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Marketo 同期ユーザがタスクを作成する場合、[!DNL Microsoft] でタスクを作成するには「**[!UICONTROL 期限]**」が必須フィールドです。 この値を入力しない場合、Marketo でデフォルトの 5 日が自動入力されます。

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>「フローアクション」でタスクに対して指定された「ステータス」フィールドにより、[!DNL Microsoft] の「ステータス理由」フィールドが更新されます。

>[!TIP]
>
>**[!UICONTROL 件名]**&#x200B;と&#x200B;**[!UICONTROL 説明]**&#x200B;で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。 詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}を参照してください。
