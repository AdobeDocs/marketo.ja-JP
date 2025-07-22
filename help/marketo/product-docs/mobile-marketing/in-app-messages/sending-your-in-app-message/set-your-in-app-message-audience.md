---
unique-page-id: 10617431
description: アプリ内メッセージオーディエンスの設定 - Marketo ドキュメント - 製品ドキュメント
title: アプリ内メッセージオーディエンスの設定
exl-id: 696ae5b6-7063-41bc-bcef-27879182ff1e
feature: Mobile Marketing
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 81%

---

# アプリ内メッセージオーディエンスの設定 {#set-your-in-app-message-audience}

最初の手順は、アプリ内メッセージを受け取るユーザーを決定することです。スマートリストを設定する必要があります。

1. 「**[!UICONTROL スマートリストを編集]**」をクリックします。

   ![](assets/image2016-5-9-15-3a15-3a7.png)

1. スマートリストの「**[!UICONTROL モバイルアプリのアクティビティがある]**」トリガーが自動的に入力されます。 ドロップダウンをクリックし、メッセージを配置するアプリを選択します。

   ![](assets/image2016-5-9-15-3a18-3a10.png)

   >[!NOTE]
   >
   >現在、アプリ内メッセージプログラムでは「モバイルアプリ」フィールドでの複数の値はサポートされていません。

1. 「**[!UICONTROL アプリを開く]**」はデフォルトのアクション設定ですが、既に設定済みの任意のカスタムイベントを選択できます。

   ![](assets/image2016-5-9-15-3a20-3a23.png)

   >[!NOTE]
   >
   >デフォルトのトリガー（[!UICONTROL &#x200B; アプリを開く &#x200B;]）と、デベロッパーがコードに追加したカスタムトリガーが、[!UICONTROL &#x200B; アクション &#x200B;] セレクターに自動的に表示されます。 カスタムイベントがない場合は、デベロッパーに問い合わせて、カスタムイベントがアプリに追加されていることを確認してください。カスタムイベントのコーディングと承認プロセスの完了には時間がかかる場合があります。詳しくは、[この記事](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md)を参照してください。

1. 必要な場合、**[!UICONTROL モバイルアプリアクティビティあり]**&#x200B;トリガーでは制約を利用できます。

   ![](assets/image2016-5-9-15-3a22-3a27.png)

1. スマートリストにフィルターを追加して、アプリ内メッセージの受信者を制限できます。この例では、**[!UICONTROL 獲得日]** フィルターを使用して、2016 年 6 月 9 日に取得されたユーザーのみがアプリ内メッセージを送信します。

   ![](assets/image2016-5-9-15-3a26-3a2.png)

1. アプリ内メッセージコントロールパネルに戻ります。ドロップダウンで表示の制限を設定します。

   ![](assets/image2016-5-9-15-3a30-3a35.png)

   >[!NOTE]
   >
   >デフォルトの表示制限は&#x200B;**[!UICONTROL セッションごとに 1 回]**&#x200B;です。受信者が応答した後にメッセージの表示を停止する場合は、「**[!UICONTROL タップされるまで毎回]**」を選択します。受信者が何を実行しても毎回表示するには、「**[!UICONTROL 毎回]**」を選択します。

   ![](assets/image2016-5-9-15-3a32-3a6.png)

お疲れさまでした。オーディエンスが設定されました。青いバーと緑のチェックマークを獲得しました。

次に、[アプリ内メッセージを選択](/help/marketo/product-docs/mobile-marketing/in-app-messages/sending-your-in-app-message/select-your-in-app-message.md)します。
