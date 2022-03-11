---
description: メールボットアクティビティのフィルター - Marketo ドキュメント - 製品ドキュメント
title: メールボットアクティビティのフィルター
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 57%

---

# メールボットアクティビティのフィルター {#filtering-email-bot-activity}

メールボットアクティビティによって、メールの開封数とクリック数のデータが誤って水増しされる場合があります。これは次のように修正できます。

>[!NOTE]
>
>[IAB/ABC International Spiders and Bots List](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/) を使用すると、このリストに記載されている IP またはユーザーエージェントを含むすべての開封／クリックアクティビティは、ボットアクティビティとして識別され、Marketo にはログインされません。

1. 「**管理者**」をクリックします。

   ![](assets/filtering-email-bot-activity-1.png)

1. 「**メール**」をクリックします。

   ![](assets/filtering-email-bot-activity-2.png)

1. 「**ボットアクティビティ**」タブをクリックします。

   ![](assets/filtering-email-bot-activity-3.png)

1. スライダーをクリックして有効にします。 **ボットアクティビティをフィルタリング**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>ボットアクティビティをログに記録するかどうかを別々に選択できます。 選択しない場合は、誤った数字が除外されるので、電子メールの開封数とクリック数がドロップされる場合があります。

**オプションの手順**:この機能を無効にするには、スライダーの選択を解除します。 無効にした場合、「過去 90 日間のボットアクティビティ」データはリセット&#x200B;**されません**。

>[!TIP]
>
>「ボットアクティビティです」ブール値（はい/いいえ）を介して、または適用可能なフィルター/トリガー制約で、スマートリストのボットアクティビティデータを活用します。
