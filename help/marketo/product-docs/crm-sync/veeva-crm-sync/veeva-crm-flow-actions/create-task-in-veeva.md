---
description: Veeva でのタスクの作成 — Marketoドキュメント — 製品ドキュメント
title: Veeva でタスクを作成
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 60%

---

# Veeva でタスクを作成 {#create-task-in-veeva}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

![](assets/create-task-in-veeva-1.png)

>[!NOTE]
>
>Marketo同期ユーザーがタスクを作成しているとき、 **期限** は、Veeva でタスクを作成するための必須フィールドです。 この値がない場合、Marketo でデフォルトの 5 日が自動入力されます。

デフォルトでは、フローステップは次のようになります。

![](assets/create-task-in-veeva-2.png)

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/create-task-in-veeva-3.png)

>[!TIP]
>
>件名と説明で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。詳しくは、 [フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md){target=&quot;_blank&quot;} を参照してください。
