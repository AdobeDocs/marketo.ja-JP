---
unique-page-id: 11376159
description: プッシュ通知とアプリ内メッセージを作成する前に、Marketo Docs — 製品ドキュメントを参照してください。
title: プッシュ通知とアプリ内メッセージを作成する前に
translation-type: tm+mt
source-git-commit: d88fb92a00e4c20509617e6ef8b2e51b66cc085b
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# プッシュ通知とアプリ内メッセージを作成する前に {#before-you-create-push-notifications-and-in-app-messages}

プッシュ通知やアプリ内メッセージの作成は難しくありませんが、開始を行うには、準備が整っている必要があります。 マーケティング担当者およびモバイルアプリの開発者は、次の手順に従って必要な統合を準備する必要があります。

1. まず、マーケティング担当者がモバイルアプリを [追加します](add-a-mobile-app.md)
1. 次に、マーケティング担当者がコードスニペットを開発者に [送信します](send-sdk-code-to-a-developer.md)
1. 開発者はSDKをダウンロードし、 [Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) またはiOS用のスニペットやその他のメソッドを含めます [。](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)
1. デフォルトでは、アプリを開くとアプリ内メッセージがトリガーされます。 特定のページが表示されたり、特定のボタンが押されたりした場合など、他のイベント向けにメッセージをトリガーする場合は、開発者はカスタムイベントをコードに追加する必要があります(下の「アプリ内メッセージの [カスタムイベント](#CustomEvents) 」を参照)。
1. 開発者は、Androidの場合はServer APIキーとプロジェクト番号、iOSの場合は証明書 [](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/)[](http://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/) とパスワードを生成し、Marketor管理者に送信します
1. マーケティング担当者は、サーバーAPIキー(Android) [または証明書(iOS)](configure-mobile-app-android-push-access.md) を使用して [、プッシュ通知アクセスを設定します](configure-mobile-app-ios-push-access.md)

>[!TIP]
>
>マーケティング担当者は、プッシュ設定が検証済みかどうかを簡単に確認できます。 行 [け](verify-push-configuration.md)。

## アプリ内メッセージのカスタムイベント {#custom-events-for-in-app-messages}

アプリ内メッセージの場合、表示トリガーは、デフォルトで **「アプリを開く** 」に設定されます。 アプリ内メッセージの表示をトリガーするカスタムイベント( **買い物かごへの追加クリック数、**&#x200B;表示設定ページなど ****)を使用する場合は、必要なイベントのリストを作成し、モバイルアプリの開発者に提供します。 次に、開発者はカスタムイベントをコードに追加します。 承認された後は、オーディエンスの設定時に、表示トリガーとして表示されます。 **注意**:カスタムイベントコーディングの承認プロセスの完了には、時間がかかる場合があります。

アプリ内メッセージとプッシュ通知の準備が完了したら、始める時間です。

>[!NOTE]
>
>**関連記事**
>
>* [アプリ内メッセージの作成](http://docs.marketo.com/display/docs/create+an+in-app+message)
   >
   >
* [プッシュ通知の作成](../../../product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

>



