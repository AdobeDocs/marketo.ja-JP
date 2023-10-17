---
unique-page-id: 37356429
description: Microsoft でのタスクの作成 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft でのタスクの作成
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 67%

---

# Microsoft でのタスクの作成 {#create-task-in-microsoft}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

Microsoftでタスクを作成では、「 [!DNL Microsoft].

>[!NOTE]
>
>このフローステップは、スマートキャンペーンで、フィルターではなく、_トリガーで使用された場合にのみ機能_&#x200B;します。

デフォルトでは、フローステップは次のようになります。

![](assets/msd1.png)

>[!NOTE]
>
>Marketo同期ユーザーがタスクを作成しているとき、 **[!UICONTROL 期限]** は、タスクを作成するための必須フィールドです。 [!DNL Microsoft]. この値を入力しない場合、Marketo でデフォルトの 5 日が自動入力されます。

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/msd2.png)

>[!NOTE]
>
>「フロー・アクション」でタスクに対して指定された「ステータス」フィールドが、「ステータスの理由」フィールド ( [!DNL Microsoft].

>[!TIP]
>
>**[!UICONTROL 件名]**&#x200B;と&#x200B;**[!UICONTROL 説明]**&#x200B;で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}を参照してください。
