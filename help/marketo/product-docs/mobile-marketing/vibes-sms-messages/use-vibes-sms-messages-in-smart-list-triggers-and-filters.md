---
unique-page-id: 11378871
description: スマートリストのトリガーとフィルターでの Vibes SMS メッセージの使用 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストトリガーとフィルターでの Vibes SMS メッセージの使用
exl-id: 9a629a39-fddc-4ec5-b1c5-d5053d676594
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '281'
ht-degree: 100%

---

# スマートリストトリガーとフィルターでの Vibes SMS メッセージの使用 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

[Vibes SMS メッセージを作成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)した後、スマートキャンペーン内でスマートリストトリガーとフィルターを使用して、メリットを得ることができます。手順は以下のとおりです。

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. SMS アセットを使用するスマートキャンペーンを選択します。よく知られている&#x200B;**フォームを入力**&#x200B;などのトリガーをドラッグします。

   ![](assets/fills-out-form-pull-over.jpg)

## SMS トリガー {#sms-triggers}

他の SMS トリガーもあります。SMS トリガーは、Vibes サービスが有効な場合にのみ表示されます。

![](assets/new-sms-search2.png)

以下に、いくつかの例を示します。

「SMS メッセージのバウンス」トリガーは、SMS メッセージがバウンスしたときにメールの送信などのフローを開始します。

![](assets/sms-message-bounces-real.jpg)

**Vibes リストの購読**&#x200B;トリガーは、ユーザーが購読するとフローを開始します。

![](assets/subscribes-to-vibes-list-real.jpg)

**SMS メッセージ内のリンクをクリック**&#x200B;トリガーは、ユーザーが SMS メッセージ内のリンクをクリックすると、フローを開始します。

![](assets/clicks-link-in-sms-message.jpg)

## SMS フィルター {#sms-filters}

また、スマートリストで Vibes フィルターを使用することもできます。**Vibes リストに購読済み**&#x200B;フィルターは、*一度でも* Vibes を購読していたことのあるすべての人を検索します。削除されたリードがフローから除外されても、登録解除済みのリードと削除済みのリードの両方が含まれます。このフィルターは、レポートに最適です。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

これに対して、**Vibes リストのメンバー**&#x200B;フィルターは、現在 Vibes を購読している&#x200B;_すべて_&#x200B;のユーザーを検索するので、スマートキャンペーンまたはリストでの使用に最も適しています。

![](assets/image001.png)

>[!NOTE]
>
>すべての SMS フィルターには、**アクティビティの日付**&#x200B;制約がデフォルトで設定されています。

スマートリストで Vibes のトリガーとフィルターを設定した後は、[フローを定義](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md)できます。

>[!MORELIKETHIS]
>
>* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [フィルターを検索してスマートリストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)

