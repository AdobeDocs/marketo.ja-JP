---
unique-page-id: 11378871
description: スマートリストのトリガーとフィルターでVibes SMSメッセージを使用する — Marketto Docs — 製品ドキュメント
title: スマートリストのトリガーとフィルターでVibe SMSメッセージを使用する
translation-type: tm+mt
source-git-commit: 06e0f5489e6375a97e2fe77834bf45fa41f23ea6
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---


# スマートリストトリガーとフィルターでVibe SMSメッセージを使用{#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

[Vibes SMSメッセージ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)を作成した後、スマートキャンペーン内でスマートリストトリガーとフィルターを使用して、メリットを得る必要があります。 これが方法です。

1. 「マイマーケット」で、「**マーケティングアクティビティ**」をクリックします。

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. SMSアセットを使用するスマートキャンペーンを選択します。 人気の&#x200B;**「Fills Out Form**」などのトリガー上にドラッグします。

   ![](assets/fills-out-form-pull-over.jpg)

## SMSトリガー{#sms-triggers}

その他のSMSトリガーを使用できます。 SMSトリガーは、Vibesサービスが有効な場合にのみ表示されます。

![](assets/new-sms-search2.png)

次に例を示します。

SMSメッセージバウンストリガーは、SMSメッセージがバウンスしたときに電子メールの送信など、フローを開始します。

![](assets/sms-message-bounces-real.jpg)

**Subscribes to Vibesリスト**&#x200B;トリガーは、訪問者が購読するとフローを開始します。

![](assets/subscribes-to-vibes-list-real.jpg)

**Clicks Link in SMS Message**&#x200B;トリガーは、SMSメッセージ内のリンクをクリックするとフローを開始します。

![](assets/clicks-link-in-sms-message.jpg)

## SMSフィルター{#sms-filters}

また、スマートリストでVibeフィルターを使用することもできます。 **Subscribed to Vibesリスト**&#x200B;フィルターは、*ever*&#x200B;がVibesをサブスクライブしている人を見つけます。 これには、削除されたユーザーがフローから除外されていても、登録解除されたユーザーと削除されたユーザーの両方が含まれます。 このフィルタはレポートに最適です。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

一方、**Member of Vibesリスト**&#x200B;フィルターは、Vibesに現在登録されている&#x200B;_any_&#x200B;を探し、スマートキャンペーンやリストでの使用に最適です。

![](assets/image001.png)

>[!NOTE]
>
>すべてのSMSフィルターには、既定で&#x200B;**アクティビティ**&#x200B;の日付制約が含まれます。

スマートリストでVibesのトリガーとフィルターを設定した後、[フロー](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md)を定義できます。

>[!MORELIKETHIS]
>
>* [スマートキャンペーンのスマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [スマート・リストの検索と追加フィルター](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

