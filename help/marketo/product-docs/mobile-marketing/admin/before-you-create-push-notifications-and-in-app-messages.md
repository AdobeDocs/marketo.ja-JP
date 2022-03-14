---
unique-page-id: 11376159
description: プッシュ通知とアプリ内メッセージを作成する前に — Marketo ドキュメント — 製品ドキュメント
title: プッシュ通知およびアプリ内メッセージを作成する前に
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '352'
ht-degree: 100%

---

# プッシュ通知およびアプリ内メッセージを作成する前に {#before-you-create-push-notifications-and-in-app-messages}

プッシュ通知とアプリ内メッセージの作成は困難ではありませんが、開始する前に準備を整えておく必要があります。Marketo 管理者およびモバイルアプリデベロッパーは、必要な統合を準備するために、以下の手順に従う必要があります。

1. まず、Marketo 管理者が[モバイルアプリを追加](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md)します。

1. Marketo 管理者が[コードスニペットをデベロッパーに送信](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md)します。

1. デベロッパーが、SDK をダウンロードし、[Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android/) または [iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios/) 用のスニペットと他のメソッドを含めます。

1. デフォルトでは、アプリを開いたときにアプリ内メッセージがトリガーされます。特定のページが表示されたり、特定のボタンが押されたりした場合など、他のイベントに関するメッセージをトリガーするには、デベロッパーがカスタムイベントをコードに追加する必要があります（[アプリ内メッセージのカスタムイベント](#CustomEvents)を参照）。

1. デベロッパーは、[Server API キーとプロジェクト番号](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-android/)（Android）または[証明書とパスワード](https://developers.marketo.com/documentation/mobile/enabling-push-notifications-on-ios/)（iOS）を生成し、Marketo 管理者に送信します。

1. Marketo 管理者が [Server API キー（Android）](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) または[証明書（iOS）](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)を使用してプッシュ通知アクセスを設定します。

>[!TIP]
>
>Marketo 管理者はプッシュ設定が検証されたかどうかを簡単に確認できます。[こちら](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md)にアクセスしてください。

## アプリ内メッセージのカスタムイベント {#custom-events-for-in-app-messages}

アプリ内メッセージの場合、デフォルトの表示トリガーは&#x200B;**アプリを開く**&#x200B;に設定されています。任意のカスタムイベントを使用してアプリ内メッセージの表示をトリガー化する場合（例：**買い物かごに追加をクリック**、**設定ページを表示**）、目的のイベントのリストを作成し、モバイルアプリデベロッパーに提供します。次に、デベロッパーはカスタムイベントをコードに追加します。承認されると、オーディエンスの設定時に表示トリガーとして表示されます。**注意**：カスタムイベントコーディングの承認プロセスの完了には、時間がかかる場合があります。

アプリ内メッセージおよびプッシュ通知の準備がすべて完了したら、開始します。

>[!MORELIKETHIS]
>
>* [アプリ内メッセージの作成](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [プッシュ通知の作成](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)

