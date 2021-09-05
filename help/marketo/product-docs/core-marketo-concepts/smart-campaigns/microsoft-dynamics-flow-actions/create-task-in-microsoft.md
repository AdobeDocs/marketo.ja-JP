---
unique-page-id: 37356429
description: Microsoft でのタスクの作成 - Marketo ドキュメント - 製品ドキュメント
title: Microsoft でのタスクの作成
exl-id: b9ae425b-edf1-4aae-92f4-e7c6cf647cdc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '171'
ht-degree: 100%

---

# Microsoft でのタスクの作成 {#create-task-in-microsoft}

マーケターは、取引の成立に関して営業を支援できる情報を持っています。タスクを作成して、タスクの実行内容と実行タイミングを営業に知らせることができます。

「Microsoft でタスクを作成」は、Microsoft で人物（リードまたは連絡先）に関連するアクティビティの下にタスクを作成します。

>[!NOTE]
>
>このフローステップは、スマートキャンペーンで、フィルターではなく、**トリガーで使用された場合にのみ機能**&#x200B;します。

デフォルトでは、フローステップは次のようになります。

![](assets/msd1.png)

>[!NOTE]
>
>Marketo 同期ユーザーがタスクを作成する場合、Microsoft でタスクを作成するには「**期限**」が必須フィールドです。この値を入力しない場合、Marketo でデフォルトの 5 日が自動入力されます。

すべてのフィールドをカスタマイズして、目的のタスクを作成します。

![](assets/msd2.png)

>[!NOTE]
>
>「フローアクション」でタスクに対して指定された「ステータス」フィールドにより、Microsoft の「ステータス理由」フィールドがアップデートされます。

>[!TIP]
>
>**件名**&#x200B;と&#x200B;**説明**&#x200B;で、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}` を使用できます。詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)を参照してください。
