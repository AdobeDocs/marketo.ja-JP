---
unique-page-id: 37356429
description: Microsoft - Marketto Docs — 製品ドキュメントでタスクを作成する
title: Microsoftでタスクを作成する
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Microsoftでタスクを作成する {#create-task-in-microsoft}

マーケティング担当者は、掘り出し物の成約を支援する情報を持っています。 タスクを作成して、何をすべきか、いつやるべきかを知らせることができます。

「Microsoftでタスクを作成」は、Microsoftの個人（リードまたは連絡先）に関連するアクティビティの下にタスクを作成します。

>[!NOTE]
>
>このフロー手順は、スマートキャンペーンでトリガーと共に使用した **場合にの**&#x200B;み機能します。フィルターと共に使用する場合は機能しません。

デフォルトでは、フローステップは次のようになります。   ![](assets/msd1.png)

>[!NOTE]
>
>Marketor Sync Userがタスクを作成する場合、Microsoftでタスクを作成するには、「**Due In **」が必須フィールドです。 値を入力しない場合、マーケティング担当者はデフォルトで5日間を入力します。

すべてのフィールドをカスタマイズして、希望どおりにタスクを作成します。   ![](assets/msd2.png)

>[!NOTE]
>
>フローアクションでタスクに対して指定された「ステータス」フィールドで、次のフィールドを更新します。Microsoftの「ステータス理由」。

>[!TIP]
>
>Subject `{{lead.tokens}}``{{company.tokens}}`and `{{campaign.tokens}}` Descriptionで、、、、および `{{system.tokens}}`********&#x200B;を使用できます。 詳細は、「フロー手順の [トークン](http://docs.marketo.com/x/c4AR) 」を参照してください。

