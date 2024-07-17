---
unique-page-id: 37356429
description: Microsoft でのタスクの作成 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft でのタスクの作成
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 67%

---

# Microsoft でのタスクの作成 {#create-task-in-microsoft}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

Microsoftのタスクを作成を使用すると、[!DNL Microsoft] のユーザー（リードまたは連絡先）に関連するアクティビティの下にタスクを作成できます。

>[!NOTE]
>
>このフローステップは、スマートキャンペーンで、フィルターではなく、_トリガーで使用された場合にのみ機能_&#x200B;します。

デフォルトでは、フローステップは次のようになります。

![](assets/create-task-in-microsoft-1.png)

>[!NOTE]
>
>Marketo Sync User がタスクを作成する場合、[!DNL Microsoft] で作成するタスクには **[!UICONTROL 期限]** が必須フィールドになります。 この値を入力しない場合、Marketo でデフォルトの 5 日が自動入力されます。

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/create-task-in-microsoft-2.png)

>[!NOTE]
>
>フローアクションでタスクに指定された「ステータス」フィールドは、[!DNL Microsoft] の「ステータス理由」フィールドを更新します。

>[!TIP]
>
>**[!UICONTROL 件名]**&#x200B;と&#x200B;**[!UICONTROL 説明]**&#x200B;で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}を参照してください。
