---
description: スマートリストのトリガーとフィルターでの Vibes SMS メッセージの使用 - Marketo ドキュメント - 製品ドキュメント
title: スマートリストトリガーとフィルターでの Vibes SMS メッセージの使用
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 46%

---

# スマートリストトリガーとフィルターでの Vibes SMS メッセージの使用 {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

新規ドキュメント

後で [Vibes SMS メッセージを作成する](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}スマートリストのトリガーとフィルターをスマートキャンペーン内で使用して、メリットを得ることができます。 手順は以下のとおりです。

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. SMS アセットを使用するスマートキャンペーンを選択します。 トリガー上にドラッグ。 この例では、 **フォームの入力**.

   ![](assets/fills-out-form-pull-over.jpg)

## SMS トリガー {#sms-triggers}

他の SMS トリガーもあります。SMS トリガーは、Vibes サービスが有効な場合にのみ表示されます。

SMS メッセージを送信：

* マーケティング活動/新しいスマートキャンペーンの選択
   * スマートリスト > Vibes リストフィルターを選択して論理を修正 > Vibes リスト：ドロップダウンからリストを選択します（Vibes プラットフォームから同期するモバイルデータベースリスト）。
      * セグメント化を絞り込み、1 つのキャンペーン内で SMS と E メールのフィルターとトリガーを利用できます。
      * Vibes フィルタ： Vibes リストへの配信登録と Vibes リストのメンバー登録 — ロジックはメールと一致します
         * Vibes リストの配信登録 — Vibes リストを配信登録した参加者が、配信登録を解除された場合でも、その Vibes リストを配信登録したことがある参加者。   — 主にクロスチャネルマーケティング活動に使用されます。
            * 注意： Vibes モバイルデータベースリストにない場合、SMS メッセージは配信停止済みのユーザーには送信されません
         * Vibes リストのメンバー — アクティブ、確認済みの購読者
         * リストに追加 — Vibes リストにこのフィルターが入力されません。これはMarketoリスト用です

![](assets/new-sms-search2.png)

以下に、いくつかの例を示します。

The **SMS メッセージのバウンス** トリガーは、SMS メッセージがバウンスしたときに E メールの送信などのフローを開始します。

![](assets/sms-message-bounces-real.jpg)

**Vibes リストの購読**&#x200B;トリガーは、ユーザーが購読するとフローを開始します。

![](assets/subscribes-to-vibes-list-real.jpg)

**SMS メッセージ内のリンクをクリック**&#x200B;トリガーは、ユーザーが SMS メッセージ内のリンクをクリックすると、フローを開始します。

![](assets/clicks-link-in-sms-message.jpg)

## SMS フィルター {#sms-filters}

また、スマートリストで Vibes フィルターを使用することもできます。**Vibes リストに購読済み**&#x200B;フィルターは、*一度でも* Vibes を購読していたことのあるすべての人を検索します。削除されたリードがフローから除外されても、登録解除済みのリードと削除済みのリードの両方が含まれます。このフィルターは、レポートに最適です。

![](assets/subscribed-to-vibes-list-filter-real.jpg)

これに対して、 **Vibes リストのメンバー** フィルター検索 _誰か_ 現在 Vibes を購読中で、スマートキャンペーンまたはリストでの使用に最も適しています。

![](assets/image001.png)

>[!NOTE]
>
>すべての SMS フィルターには、**アクティビティの日付**&#x200B;制約がデフォルトで設定されています。

スマートリストで Vibes のトリガーとフィルターを設定した後は、[フローを定義](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md)できます。

>[!MORELIKETHIS]
>
>* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [フィルターを検索してスマートリストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
