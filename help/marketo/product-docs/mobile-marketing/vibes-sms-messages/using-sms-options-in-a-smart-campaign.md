---
description: Smart Campaign での SMS オプションの使用 – Marketo ドキュメント – 製品ドキュメント
title: スマートキャンペーンでの SMS オプションの使用
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 38%

---

# スマートキャンペーンでの SMS オプションの使用 {#using-sms-options-in-a-smart-campaign}

[SMS メッセージを作成 ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"} した後は、スマートキャンペーン内でスマートリストのトリガーとフィルターを使用して、メリットを享受できます。

>[!NOTE]
>
>SMS メッセージを送信する場合は、[ 特定の記事 ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} を用意しています。

>[!PREREQUISITES]
>
>SMS トリガー/フィルターは、[Vibes サービスが有効 ](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"} になっている場合にのみ表示されます。

## SMS トリガー {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

以下に、いくつかの例を示します。

**SMS メッセージバウンス**&#x200B;トリガーは、SMS メッセージがバウンスした場合に、メールの送信などのフローを開始します。

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

これに対し、**Vibes リストのメンバー** フィルターは、現在 Vibes を購読している *任意のユーザー* を見つけ、スマートキャンペーンやリストでの使用に最も適しています。

>[!NOTE]
>
>すべての SMS フィルターには、デフォルトで **アクティビティの日付** 制約が含まれています。

## SMS フローの手順 {#sms-flow-steps}

SMS フローステップは 3 つから選択できます。

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>SMS メッセージの送信</b></td>
    <td>このフローアクションは、オプトインした Vibes 購読リストを購読しているMarketo スマートリストのユーザーにメッセージを送信します。 購読プロセスは開始されません。 <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">詳細情報</a></td>
  </tr>

<tr>
    <td style="width:20%"><b>Vibes リストに配信登録</b></td>
    <td>このフローアクションは、ユーザーが選択した Vibes 獲得キャンペーンを通じて SMS 購読プロセスを開始します。 次に、Vibes が確認メッセージを送信し、受信者は 24 時間以内に「Y」と返信してオプトインを確認する必要があります。 ユーザーがオプトインすると、関連付けられた Vibes サブスクリプションリストのメンバーになります。</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Vibes リストから配信停止</b></td>
    <td>このフローアクションは、オプトインした Vibes 購読リストから各ユーザーを購読解除します。 ユーザーがコードに「STOP」と入力すると、ユーザーのユーザーレコードが更新され、Vibes サブスクリプションリストに登録されなくなったことを反映します。</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>**Vibes リストに購読**&#x200B;および **Vibes リストから登録解除**&#x200B;フローには、異なる要件があります。**購読**&#x200B;の場合、Vibes リストと Vibes 獲得キャンペーンを選択する必要があります。**登録解除**&#x200B;の場合、Vibes リストのみが必要です。

>[!MORELIKETHIS]
>
>* [SMS メッセージの送信 ](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [スマートキャンペーン用スマートリストの定義 |トリガー](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [スマートキャンペーン用スマートリストの定義 | バッチ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
