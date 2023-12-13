---
description: スマートリストのトリガーとフィルターで SMS オプションを使用する — Marketoドキュメント — 製品ドキュメント
title: スマートリストオプションとフィルターでの SMSトリガーの使用
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 42%

---

# スマートリストオプションとフィルターでの SMSトリガーの使用 {#use-sms-options-in-smart-list-triggers-and-filters}

新規ドキュメント

後で [SMS メッセージの作成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}スマートリストのトリガーとフィルターをスマートキャンペーン内で使用して、メリットを得ることができます。

>[!PREREQUISITES]
>
>SMSトリガー/フィルターは、 [Vibes サービスが有効になっています](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## SMS トリガー {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

以下に、いくつかの例を示します。

The **SMS メッセージのバウンス** トリガーは、SMS メッセージがバウンスしたときに E メールの送信などのフローを開始します。

**Vibes リストの購読**&#x200B;トリガーは、ユーザーが購読するとフローを開始します。

**SMS メッセージ内のリンクをクリック**&#x200B;トリガーは、ユーザーが SMS メッセージ内のリンクをクリックすると、フローを開始します。

## SMS フィルター {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

スマートリストで Vibes フィルターを使用することもできます。 **Vibes リストに購読済み**&#x200B;フィルターは、*一度でも* Vibes を購読していたことのあるすべての人を検索します。削除されたリードがフローから除外されても、登録解除済みのリードと削除済みのリードの両方が含まれます。このフィルターは、レポートに最適です。

これに対して、 **Vibes リストのメンバー** フィルター検索 _誰か_ 現在 Vibes を購読中で、スマートキャンペーンまたはリストでの使用に最も適しています。

>[!NOTE]
>
>すべての SMS フィルターには、**アクティビティの日付**&#x200B;制約がデフォルトで設定されています。

スマートリストで Vibes のトリガーとフィルターを設定した後、次の操作を実行できます。 [フローの定義](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [SMS メッセージの送信](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [フィルターを検索してスマートリストに追加](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
