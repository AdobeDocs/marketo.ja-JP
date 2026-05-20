---
description: MarketoからVeevaでタスクを作成し、セールスに何をいつやるべきかを伝える方法を説明します。 「タスクを作成」フロー手順を使用して、件名、説明、期日をカスタマイズします。
title: ' [!DNL Veeva] でのタスクの作成'
exl-id: 342e45dd-2038-432d-a6b6-1740c8f0b58e
feature: Veeva CRM
TQID: https://experienceleague.adobe.com/W4zIWswN64cHyqA7oQ9iku0iMC7Q6NqIpWiAcSgvD04
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 78%

---

# [!DNL Veeva] でのタスクの作成 {#create-task-in-veeva}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。 タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Marketo 同期ユーザがタスクを作成する場合、[!DNL Veeva] でタスクを作成するには「**[!UICONTROL 期限]**」が必須フィールドです。 この値がない場合、Marketo でデフォルトの 5 日が自動入力されます。

デフォルトでは、フローステップは次のようになります。

![](assets/create-task-in-veeva-2.png)

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>[!UICONTROL 件名]と[!UICONTROL 説明]で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。 詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target="_blank"}を参照してください。
