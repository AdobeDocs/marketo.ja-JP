---
description: タスクを作成する  [!DNL Veeva] - Marketo ドキュメント – 製品ドキュメント
title: ' [!DNL Veeva] でタスクを作成'
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '115'
ht-degree: 88%

---

# [!DNL Veeva] でタスクを作成 {#create-task-in-veeva}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Marketo 同期ユーザがタスクを作成する場合、[!DNL Veeva] でタスクを作成するには「**[!UICONTROL 期限]**」が必須フィールドです。この値がない場合、Marketo でデフォルトの 5 日が自動入力されます。

デフォルトでは、フローステップは次のようになります。

![](assets/create-task-in-veeva-2.png)

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>[!UICONTROL 件名]と[!UICONTROL 説明]で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}を参照してください。
