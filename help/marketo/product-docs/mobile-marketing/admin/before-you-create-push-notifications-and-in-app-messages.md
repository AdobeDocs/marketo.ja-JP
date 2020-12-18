---
unique-page-id: 11376159
description: プッシュ通知とアプリ内メッセージを作成する前に、Marketo Docs — 製品ドキュメントを参照してください。
title: プッシュ通知とアプリ内メッセージを作成する前に
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---


# プッシュ通知とアプリ内メッセージを作成する前に{#before-you-create-push-notifications-and-in-app-messages}

プッシュ通知やアプリ内メッセージの作成は難しくありませんが、開始を行うには、準備が整っている必要があります。 マーケティング担当者およびモバイルアプリの開発者は、次の手順に従って必要な統合を準備する必要があります。

1. 最初に、マーケティング担当者[がモバイルアプリ](add-a-mobile-app.md)を追加します
1. 次に、マーケティング担当者が[開発者](send-sdk-code-to-a-developer.md)にコードスニペットを送信します
1. 開発者はSDKをダウンロードし、[Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/)または[iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)のスニペットとその他のメソッドを含めます
1. デフォルトでは、アプリを開くとアプリ内メッセージがトリガーされます。 特定のページが表示されたり、特定のボタンが押されたりした場合など、他のイベント向けにメッセージをトリガーする場合は、カスタムイベントをコードに追加する必要があります(下の[アプリ内メッセージのカスタムイベント](#CustomEvents)を参照)
1. 開発者[は、Android](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/)または[iOS](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/)の証明書とパスワード用のServer APIキーとプロジェクト番号を生成し、Marketor管理者に送信します
1. マーケティング担当者は、サーバーAPIキー(Android)](configure-mobile-app-android-push-access.md)または[を使用して、プッシュ通知アクセス[を証明書(iOS)](configure-mobile-app-ios-push-access.md)と共に設定します。

>[!TIP]
>
>マーケティング担当者は、プッシュ設定が検証済みかどうかを簡単に確認できます。 [ここ](verify-push-configuration.md)に行くだけ。

## アプリ内メッセージのカスタムイベント{#custom-events-for-in-app-messages}

アプリ内メッセージの場合、表示トリガーはデフォルトで&#x200B;**App Open**&#x200B;に設定されます。 アプリ内イベント(例：**買い物かごへのクリック数**、**表示設定ページ**&#x200B;追加へのクリック数)の表示をトリガーするには、目的のイベントのリストを作成し、モバイルアプリの開発者に提供します。 次に、開発者はカスタムイベントをコードに追加します。 承認された後は、オーディエンスの設定時に、表示トリガーとして表示されます。 **注意**:カスタムイベントコーディングの承認プロセスの完了には、時間がかかる場合があります。

アプリ内メッセージとプッシュ通知の準備が完了したら、始める時間です。

>[!MORELIKETHIS]
>
>* [アプリ内メッセージの作成](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [プッシュ通知の作成](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



