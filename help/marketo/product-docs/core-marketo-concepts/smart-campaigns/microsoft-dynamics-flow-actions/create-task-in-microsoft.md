---
unique-page-id: 37356429
description: Microsoft - Marketto Docs — 製品ドキュメントでタスクを作成する
title: Microsoftでタスクを作成する
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---


# Microsoft {#create-task-in-microsoft}でタスクを作成

マーケティング担当者は、掘り出し物の成約を支援する情報を持っています。 タスクを作成して、何をすべきか、いつやるべきかを知らせることができます。

「Microsoftでタスクを作成」は、Microsoftの個人（リードまたは連絡先）に関連するアクティビティの下にタスクを作成します。

>[!NOTE]
>
>このフローステップは、スマートキャンペーンでトリガー&#x200B;**を使用した場合にのみ機能します。フィルターではありません。**

デフォルトでは、フローステップは次のようになります。

![](assets/msd1.png)

>[!NOTE]
>
>Marketo Sync Userがタスクを作成する場合、Microsoftでタスクを作成するには、**期限**&#x200B;が必須フィールドです。 値を入力しない場合、マーケティング担当者はデフォルトで5日間を入力します。

すべてのフィールドをカスタマイズして、希望どおりにタスクを作成します。

![](assets/msd2.png)

>[!NOTE]
>
>フローアクションでタスクに対して指定された「ステータス」フィールドで、次のフィールドを更新します。Microsoftの「ステータス理由」。

>[!TIP]
>
>**件名**&#x200B;と&#x200B;**説明**&#x200B;には、`{{lead.tokens}}`、`{{company.tokens}}`、`{{campaign.tokens}}`、`{{system.tokens}}`を使用できます。 詳しくは、[フローステップのトークン](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md)を参照してください。
