---
description: SMS メッセージの送信 — Marketoドキュメント — 製品ドキュメント
title: SMS メッセージの送信
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 8%

---

# SMS メッセージの送信 {#send-a-vibes-sms-message}

You&#39;ve [SMS メッセージを作成しました](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}を送信する時間が始まりました。 バッチまたはトリガーキャンペーンで送信できます。

>[!NOTE]
>
>SMS メッセージを送信する場合：
>
>* Marketo Engage番号別のデュープ。 したがって、複数の人が同じ電話番号を持っている場合、1 人の人だけがメッセージを受け取ります（1 人の Vibes 配信登録リストのメンバーの場合）。 重複排除は、Marketoプログラムレベルではなく、Vibes 購読リストレベルでおこなわれます。
>* メッセージはブロックリストに登録されたリードやマーケティングが中断されたリードには送信されません。
>* Vibes モバイルデータベースリストにない場合、SMS メッセージは配信停止済みのユーザーには送信されません。

## バッチ SMS の送信 {#send-a-batch-sms}

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/send-an-sms-message-1.png)

1. 目的のスマートキャンペーンを見つけて選択します。

   ![](assets/send-an-sms-message-2.png)

1. 次をクリック： **スマートリスト** 」タブをクリックし、SMS のオーディエンスを定義します。 この例では、会社として「Adobe」がリストされているデータベース内の全員にを送信します。

   ![](assets/send-an-sms-message-3.png)

1. Adobe Analytics の **流量** タブ、上にドラッグ **SMS メッセージの送信**. 目的の SMS メッセージと Vibes リストをドロップダウンから選択します。

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >Vibes リストセレクターは、スマートリストで既に識別されているオーディエンスに対する追加のフィルターとして機能し、その Vibes リストに属する人のみをターゲットにします。

1. 次をクリック： **スケジュール** 「 」タブに移動し、SMS のスケジュールを設定します。

   ![](assets/send-an-sms-message-5.png)

## トリガーSMS の送信 {#send-a-trigger-sms}

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/send-an-sms-message-6.png)

1. 目的のスマートキャンペーンを見つけて選択します。

   ![](assets/send-an-sms-message-7.png)

1. 次をクリック： **スマートリスト** 「 」タブで、目的のトリガーを選択し、値を定義します。 この例では、 **フォームの入力**.

   ![](assets/send-an-sms-message-8.png)

1. Adobe Analytics の **流量** タブ、上にドラッグ **SMS メッセージの送信**. 目的の SMS メッセージと Vibes リストをドロップダウンから選択します。

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >Vibes リストセレクターは、スマートリストで既に識別されているオーディエンスに対する追加のフィルターとして機能し、その Vibes リストに属する人のみをターゲットにします。

1. 次をクリック： **スケジュール** タブ、 **有効化**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Vibes メッセージの作成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}
>* [スマートキャンペーンでの SMS オプションの使用](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
