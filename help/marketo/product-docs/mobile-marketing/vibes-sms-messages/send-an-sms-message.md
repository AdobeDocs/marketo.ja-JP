---
description: バッチまたはトリガーキャンペーンを介してSMS メッセージを送信する方法を説明します。 スマートリストを定義し、SMSを送信フローステップを追加してから、スケジュールまたはアクティブ化します。
title: SMS メッセージの送信
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 10%

---

# SMS メッセージの送信 {#send-a-vibes-sms-message}

SMS メッセージを[作成しました](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}。次に送信します。 バッチまたはトリガーキャンペーンで送ることができます。

>[!NOTE]
>
>SMS メッセージを送信する場合：
>
>* 電話番号によるMarketo Engageの重複排除。 そのため、複数のユーザーが同じ電話番号を持っている場合、1人のユーザーのみが1つのVibes サブスクリプションリストのメンバーである場合、メッセージを受け取ります。 重複排除は、Marketo プログラムレベルではなく、Vibes サブスクリプションのリストレベルで行われます。
>* メッセージはブロックリストに登録されたリードやマーケティングが中断されたリードには送信されません。
>* Vibes Mobile Database リストに登録されていないユーザーにSMS メッセージを送信することはできません。

## バッチ SMSの送信 {#send-a-batch-sms}

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/send-an-sms-message-1.png)

1. 目的のスマートキャンペーンを検索して選択します。

   ![](assets/send-an-sms-message-2.png)

1. 「**スマートリスト**」タブをクリックし、SMSのオーディエンスを定義します。 この例では、データベース内の「Adobe」が会社としてリストされている全員に送信します。

   ![](assets/send-an-sms-message-3.png)

1. **フロー** タブで、**SMS メッセージを送信**&#x200B;にドラッグします。 ドロップダウンから目的のSMS メッセージとVibes リストを選択します。

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >Vibes リストセレクターは、スマートリストですでに特定されているオーディエンスをさらにフィルターとして機能し、そのVibes リストに属するユーザーのみをターゲットにします。

1. 「**スケジュール**」タブをクリックし、SMSをスケジュールします。

   ![](assets/send-an-sms-message-5.png)

## トリガーSMSの送信 {#send-a-trigger-sms}

1. My Marketo で、**マーケティング活動**&#x200B;をクリックします。

   ![](assets/send-an-sms-message-6.png)

1. 目的のスマートキャンペーンを検索して選択します。

   ![](assets/send-an-sms-message-7.png)

1. 「**スマートリスト**」タブをクリックし、目的のトリガーを選択して、その値を定義します。 この例では、**入力フォーム**&#x200B;を使用しています。

   ![](assets/send-an-sms-message-8.png)

1. **フロー** タブで、**SMS メッセージを送信**&#x200B;にドラッグします。 ドロップダウンから目的のSMS メッセージとVibes リストを選択します。

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >Vibes リストセレクターは、スマートリストですでに特定されているオーディエンスをさらにフィルターとして機能し、そのVibes リストに属するユーザーのみをターゲットにします。

1. 「**スケジュール**」タブをクリックし、**アクティブ化**&#x200B;をクリックします。

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Vibes メッセージの作成](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [&#x200B; スマートキャンペーンでのSMS オプションの使用](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
