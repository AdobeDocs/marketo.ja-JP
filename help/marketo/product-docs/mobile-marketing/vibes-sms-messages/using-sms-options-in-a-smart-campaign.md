---
description: スマートキャンペーンでの SMS オプションの使用 — Marketoドキュメント — 製品ドキュメント
title: スマートキャンペーンでの SMS オプションの使用
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 34%

---

# スマートキャンペーンでの SMS オプションの使用 {#using-sms-options-in-a-smart-campaign}

後で [SMS メッセージの作成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message-2.md){target="_blank"}スマートリストのトリガーとフィルターをスマートキャンペーン内で使用して、メリットを得ることができます。

>[!NOTE]
>
>SMS メッセージを送信したい場合、 [特定の記事](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} それに対して

>[!PREREQUISITES]
>
>SMSトリガー/フィルターは、 [Vibes サービスが有効になっています](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## SMS トリガー {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

以下に、いくつかの例を示します。

The **SMS メッセージのバウンス** トリガーは、SMS メッセージがバウンスしたときに E メールの送信などのフローを開始します。

**Vibes リストの購読**&#x200B;トリガーは、ユーザーが購読するとフローを開始します。

**SMS メッセージ内のリンクをクリック**&#x200B;トリガーは、ユーザーが SMS メッセージ内のリンクをクリックすると、フローを開始します。

## SMS フィルター {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

**Vibes リストに購読済み**&#x200B;フィルターは、*一度でも* Vibes を購読していたことのあるすべての人を検索します。削除されたリードがフローから除外されても、登録解除済みのリードと削除済みのリードの両方が含まれます。このフィルターは、レポートに最適です。

これに対して、 **Vibes リストのメンバー** フィルター検索 _誰か_ 現在 Vibes を購読中で、スマートキャンペーンまたはリストでの使用に最も適しています。

>[!NOTE]
>
>すべての SMS フィルターには、 **アクティビティの日付** 制約をデフォルトで設定します。

## SMS フローステップ {#sms-flow-steps}

SMS のフローステップは 3 つあります。

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>SMS メッセージの送信</b></td>
    <td>このフローアクションは、オプトインした Vibes サブスクリプションリストに登録されているMarketoスマートリストの担当者にメッセージを送信します。 購読手続きは開始されません。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">詳細情報</a></td>
  </tr>

<tr>
    <td style="width:20%"><b>Vibes リストに登録</b></td>
    <td>このフローアクションは、ユーザーが選択した Vibes 獲得キャンペーンを介して SMS 購読プロセスを開始します。 Vibes が確認メッセージを送信し、受信者がオプトインを確認するには、24 時間以内に「Y」と返信する必要があります。 ユーザーがオプトインすると、関連付けられた Vibes 配信登録リストのメンバーになります。</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Vibes リストから登録解除</b></td>
    <td>このフローアクションは、オプトインした Vibes 配信登録リストから各顧客を配信停止にします。 ユーザーがコードに「STOP」と入力すると、ユーザーレコードが更新され、Vibes 配信登録リストのメンバーでなくなったことが反映されます。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>**Vibes リストに購読**&#x200B;および **Vibes リストから登録解除**&#x200B;フローには、異なる要件があります。**購読**&#x200B;の場合、Vibes リストと Vibes 獲得キャンペーンを選択する必要があります。**登録解除**&#x200B;の場合、Vibes リストのみが必要です。

>[!MORELIKETHIS]
>
>* [SMS メッセージの送信](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [スマートキャンペーン用スマートリストの定義 | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
