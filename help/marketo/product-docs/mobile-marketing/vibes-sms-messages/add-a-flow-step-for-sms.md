---
unique-page-id: 11379045
description: SMS - Marketto Docs — 製品ドキュメントのフ追加ローステップ
title: SMS追加のフローステップ
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# SMS追加のフローステップ {#add-a-flow-step-for-sms}

Marketoには、SMSスマートキャンペーンで使用できる3つのフローステップがあります。

* **SMSメッセージの送信** — このフローアクションは、ユーザーが選択したVibes購読リストを登録しているMarketoスマートリストのユーザーにメッセージを送信します。 購読プロセスは開始されません。
* **Vibesリストのサブスクライブ** — このフローアクションは、ユーザーが選択したVibes Acquisitionキャンペーンを介してSMS購読プロセスを開始します。 次に、Vibesは確認メッセージを送信します。受信者は、購読プロセスを完了するために、このメッセージに返信する必要があります。
* **Vibesリストからの登録解除** — このフローアクションは、ユーザーが選択したVibes購読リストから各個人を登録解除します。

>[!NOTE]
>
>SMSメッセージを送信する場合：
>
>* 電話番号別の重複排除。 複数の人が同じ電話番号を持っている場合、1人の人だけがメッセージを受け取ります。
>* Marketing Suspendedまたはブロックリストに加えるMarketing Suspendedのユーザーには送信されません。

>



フロー・ステップの設定に関する一般的な情報は、「スマート・キャンペーン [追加へのフロー・ステップ](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)」を参照してください。

SMSを使用する際の基本事項を以下に示します。

1. 「マーケティング」で、「 **マーケティングアクティビティ**」をクリックします。

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. SMSフローを追加するスマートキャンペーンを探します。 「 **フロー** 」タブをクリックします。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. フロー上にドラッグします(例： **Send SMS Message**)。 ドロップダウンからSMSメッセージとVibesリストを選択します。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Vibesリストセレクターは、スマートリストで既に識別されているオーディエンスに対する追加のフィルターとして機能し、そのVibesリストに属するリードのみをターゲットします。
   >
   >
   >Vibes **リストを購読** 、Vibesリストフローを **購読解除** 、要件は異なります。 「 **購読**」の場合は、VibesリストとVibes獲得キャンペーンを選択する必要があります。 「 **登録解除**」の場合は、Vibesリストのみが必要です。

