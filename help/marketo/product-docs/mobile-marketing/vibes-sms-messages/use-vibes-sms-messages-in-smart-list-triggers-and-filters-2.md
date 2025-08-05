---
description: スマートリストのトリガーとフィルターでの Vibes SMS メッセージの使用 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストトリガーとフィルターでの Vibes SMS メッセージの使用
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 46%

---

# スマートリストトリガーとフィルターでの Vibes SMS メッセージの使用 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

[Vibes SMS メッセージを作成 ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"} した後は、スマートキャンペーン内でスマートリストのトリガーとフィルターを使用して、メリットを享受できます。 手順は以下のとおりです。

1. My Marketo で、**[!UICONTROL マーケティング活動]**&#x200B;をクリックします。

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. SMS アセットを使用するスマートキャンペーンを選択します。 トリガーの上にドラッグします。 この例では、**フォームへの入力** を使用しています。

   ![](assets/fills-out-form-pull-over.jpg)

## SMS トリガー {#sms-triggers}

他の SMS トリガーもあります。SMS トリガーは、Vibes サービスが有効な場合にのみ表示されます。

SMS メッセージの送信：

* マーケティングアクティビティ /新しいスマートキャンペーンを選択
   * スマートリスト/Vibes リストを選択フィルターと適切なロジック/Vibes リスト：ドロップダウンからのリストの選択（Vibes プラットフォームから同期されるモバイルデータベースリスト）
      * セグメント化を調整し、SMS とメールのフィルターおよびトリガーを 1 つのキャンペーン内で活用できます。
      * Vibes フィルター：Vibes リストを購読 vs. Vibes リストのメンバー – ロジックがメールと一致する
         * Vibes リストを購読 – Vibes リストを購読したことがある参加者（購読解除した場合も含む）。   – 主にクロスチャネルマーケティング活動に利用
            * 注意：SMS メッセージは、Vibes モバイルデータベース リストに登録されていない場合、登録を解除したユーザーには送信されません
         * バイブリストのメンバー – アクティブで確認済みのサブスクライバー
         * リストに追加 – バイブリストはこのフィルターを使用しません。これはMarketo リスト用です

![](assets/new-sms-search2.png)

以下に、いくつかの例を示します。

**SMS メッセージバウンス**&#x200B;トリガーは、SMS メッセージがバウンスした場合に、メールの送信などのフローを開始します。

![](assets/sms-message-bounces-real.jpg)

**[!UICONTROL Vibes リストの購読]**&#x200B;トリガーは、ユーザーが購読するとフローを開始します。

![](assets/subscribes-to-vibes-list-real.jpg)

**[!UICONTROL SMS メッセージ内のリンクをクリック]**&#x200B;トリガーは、ユーザーが SMS メッセージ内のリンクをクリックすると、フローを開始します。

![](assets/clicks-link-in-sms-message.jpg)

## SMS フィルター {#sms-filters}

また、スマートリストで Vibes フィルターを使用することもできます。**[!UICONTROL Vibes リストに購読済み]**&#x200B;フィルターは、*一度でも* Vibes を購読していたことのあるすべての人を検索します。削除されたリードがフローから除外されても、登録解除済みのリードと削除済みのリードの両方が含まれます。このフィルターは、レポートに最適です。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

これに対し、**Vibes リストのメンバー** フィルターは、現在 Vibes を購読している *任意のユーザー* を見つけ、スマートキャンペーンやリストでの使用に最も適しています。

![](assets/image001.png)

>[!NOTE]
>
>すべての SMS フィルターには、**[!UICONTROL アクティビティの日付]**&#x200B;制約がデフォルトで設定されています。

スマートリストで Vibes のトリガーとフィルターを設定した後は、[フローを定義](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md)できます。

>[!MORELIKETHIS]
>
>* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [フィルターを検索してスマートリストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
