---
unique-page-id: 11378871
description: スマートリストトリガーおよびフィルターでのVibes SMSメッセージの使用 — Marketto Docs — 製品ドキュメント
title: スマートリストトリガおよびフィルターでのVibe SMSメッセージの使用
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# スマートリストトリガーとフィルターでVibe SMSメッセージを使用{#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

[VibesのSMSメッセージ](create-a-vibes-sms-message.md)を作成した後、スマートリストトリガーとフィルターをスマートキャンペーン内で使用して、メリットを得る必要があります。 これが方法です。

1. 「マイマーケット」で、「**マーケティングアクティビティ**」をクリックします。

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. SMSアセットを使用するスマートキャンペーンを選択します。 トリガーの上にドラッグします。例えば、人気の&#x200B;**Fills Out Form**&#x200B;などです。

   ![](assets/fills-out-form-pull-over.jpg)

## SMSトリガ{#sms-triggers}

他のSMSトリガーを使用できます。 SMSトリガは、Vibesサービスが有効な場合にのみ表示されます。

![](assets/new-sms-search2.png)

次に例を示します。

SMSメッセージバウンストリガは、SMSメッセージがバウンスしたときに、電子メールの送信など、フローを開始します。

![](assets/sms-message-bounces-real.jpg)

**Subscribes to Vibesリスト**&#x200B;トリガーは、訪問者が購読するとフローを開始します。

![](assets/subscribes-to-vibes-list-real.jpg)

[** Clicks Link in SMS Message**]トリガは、ユーザーがSMSメッセージ内のリンクをクリックするとフローを開始します。

![](assets/clicks-link-in-sms-message.jpg)

## SMSフィルター{#sms-filters}

また、スマートリストでVibeフィルターを使用することもできます。 **Subscribed to Vibesリスト**&#x200B;フィルターは、*ever*&#x200B;がVibesをサブスクライブしている人を見つけます。 これには、削除されたユーザーがフローから除外されていても、登録解除されたユーザーと削除されたユーザーの両方が含まれます。 このフィルタはレポートに最適です。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

一方、**Member of Vibesリスト&#x200B;**filter**&#x200B;は、**** any *****currently*がVibesに登録しているのを検出し、スマートキャンペーンやリストでの使用に最適です。**

![](assets/image001.png)

>[!NOTE]
>
>すべてのSMSフィルターには、既定で&#x200B;**アクティビティ**&#x200B;の日付制約が含まれます。

スマートリストでVibesトリガーとフィルターを設定した後、[フロー](add-a-flow-step-for-sms.md)を定義できます。

>[!MORELIKETHIS]
>
>* [スマートキャンペーンのスマートリストの定義 |トリガー](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [スマート・リストの検索と追加フィルター](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [SMS追加のフローステップ](add-a-flow-step-for-sms.md)

>



