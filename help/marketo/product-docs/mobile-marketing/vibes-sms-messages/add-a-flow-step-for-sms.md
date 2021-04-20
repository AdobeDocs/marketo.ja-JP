---
unique-page-id: 11379045
description: SMS -追加Marketoドキュメント — 製品ドキュメントのフローステップ
title: SMS追加のフローステップ
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# SMS追加のフローステップ{#add-a-flow-step-for-sms}

Marketoには、SMSスマートキャンペーンで使用できる3つのフローステップがあります。

* **SMSメッセージの送信**  — このフロー操作は、ユーザーが選択したVibes購読リストを登録しているMarketoスマートリストのユーザーにメッセージを送信します。購読プロセスは開始されません。
* **Vibesリストに登録**  — このフローアクションは、ユーザーが選択したVibes Acquisitionキャンペーンを介してSMS購読プロセスを開始します。次に、Vibesは確認メッセージを送信します。受信者は、購読プロセスを完了するために、このメッセージに返信する必要があります。
* **Vibesリストからの登録解除**  — このフロー・アクションは、ユーザーが選択したVibes購読リストから各個人を登録解除します。

>[!NOTE]
>
>SMSメッセージを送信する場合：
>
>* Marketoは電話番号別に重複を排除しました。 複数の人が同じ電話番号を持っている場合、1人の人だけがメッセージを受け取ります。
>* Marketoは、ブロックリストに加えるMarketing SuspendedまたはMarketing Suspendedのユーザーに送信しません。


フローステップの設定に関する一般的な情報については、「[スマートキャンペーンへ追加のフローステップ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)」を参照してください。

SMSを使用する際の基本事項を以下に示します。

1. マイMarketoで、「**マーケティングアクティビティ**」をクリックします。

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. SMSフローを追加するスマートキャンペーンを探します。 「**フロー**」タブをクリックします。

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. フロー上にドラッグします（例：**Send SMS Message**）。 ドロップダウンからSMSメッセージとVibesリストを選択します。

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Vibesリストセレクターは、スマートリストで既に識別されているオーディエンスに対する追加のフィルターとして機能し、そのVibesリストに属するリードのみをターゲットします。
   >
   >**Subscribe to Vibesリスト**&#x200B;と&#x200B;**Unsubscribe from Vibesリスト**&#x200B;のフローは、異なる要件を持ちます。 **購読**&#x200B;の場合、VibesリストとVibes獲得キャンペーンを選択する必要があります。 **登録解除**&#x200B;の場合は、Vibesリストのみが必要です。
