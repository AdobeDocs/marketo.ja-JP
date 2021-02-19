---
unique-page-id: 11376159
description: プッシュ通知とアプリ内メッセージを作成する前に、Marketo Docs — 製品ドキュメントを参照してください。
title: プッシュ通知とアプリ内メッセージを作成する前に
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---


# プッシュ通知とアプリ内メッセージを作成する前に{#before-you-create-push-notifications-and-in-app-messages}

プッシュ通知やアプリ内メッセージの作成は難しくありませんが、開始を行うには、準備が整っている必要があります。 マーケティング担当者およびモバイルアプリの開発者は、次の手順に従って必要な統合を準備する必要があります。

1. まず、マーケティング担当者[がモバイルアプリ](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md)を追加します。

1. 次に、マーケティング担当者は、コードスニペットを[開発者](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md)に送信します。

1. 開発者はSDKをダウンロードし、[Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/)または[iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/)のスニペットとその他のメソッドを含めます。

1. デフォルトでは、アプリを開くとアプリ内メッセージがトリガーされます。 特定のページが表示されたり、特定のボタンが押されたりした場合など、他のイベント向けにメッセージをトリガーする場合は、カスタムイベントをコードに追加する必要があります(下の[アプリ内メッセージのカスタムイベント](#CustomEvents)を参照)。

1. 開発者[は、Android](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/)または[iOS](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/)の認証とパスワード用のServer APIキーとプロジェクト番号を生成し、Marketor管理者に送信します。

1. マーケティング担当者は、サーバーAPIキー(Android)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md)または[を使用して、プッシュ通知アクセス[を証明書(iOS)](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)を設定します。

>[!TIP]
>
>マーケティング担当者は、プッシュ設定が検証済みかどうかを簡単に確認できます。 [ここ](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md)に行くだけ。

## アプリ内メッセージのカスタムイベント{#custom-events-for-in-app-messages}

アプリ内メッセージの場合、表示トリガーはデフォルトで&#x200B;**App Open**&#x200B;に設定されます。 アプリ内メッセージの表示のトリガーにカスタムイベントを使用する場合(例：**買い物かごへのクリック数**、**表示設定ページ**)、必要なイベントのリストを作成し、モバイルアプリの開発者に提供します。 次に、開発者はカスタムイベントをコードに追加します。 承認されたユーザーは、オーディエンスの設定時に表示トリガーとして表示されます。 **注意**:カスタムイベントコーディングの承認プロセスの完了には、時間がかかる場合があります。

アプリ内メッセージとプッシュ通知の準備が完了したら、始める時間です。

>[!MORELIKETHIS]
>
>* [アプリ内メッセージの作成](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
   >
   >
* [プッシュ通知の作成](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

