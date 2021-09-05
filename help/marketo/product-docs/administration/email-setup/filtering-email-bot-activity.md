---
description: メールボットアクティビティのフィルター - Marketo ドキュメント - 製品ドキュメント
title: メールボットアクティビティのフィルター
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: ht
source-wordcount: '136'
ht-degree: 100%

---

# メールボットアクティビティのフィルター {#filtering-email-bot-activity}

メールボットアクティビティによって、メールの開封数とクリック数のデータが誤って水増しされる場合があります。これは次のように修正できます。

>[!NOTE]
>
>[IAB/ABC International Spiders and Bots List](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/) を使用すると、このリストに記載されている IP またはユーザーエージェントを含むすべての開封／クリックアクティビティは、ボットアクティビティとして識別され、Marketo にはログインされません。

1. 「**管理**」をクリックします。

   ![](assets/filtering-email-bot-activity-1.png)

1. 「**メール**」をクリックします。

   ![](assets/filtering-email-bot-activity-2.png)

1. 「**ボットアクティビティ**」タブをクリックします。

   ![](assets/filtering-email-bot-activity-3.png)

1. 「**メールボットアクティビティのフィルターを有効にする**」チェックボックスをオンにします。

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>この機能を有効にすると、不正な数は除外されるので、メールの開封数とクリック数が減少する場合があります。

**オプションの手順**：チェックボックスをオフにすればこの機能は無効になります。無効にした場合、「過去 90 日間のボットアクティビティ」データはリセット&#x200B;**されません**。
