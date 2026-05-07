---
unique-page-id: 11376159
description: プッシュメッセージとアプリ内メッセージを作成する前に、何を設定すればよいかを把握します。 管理者と開発者の手順、SDK、カスタムイベントのガイダンスを確認します。
title: プッシュ通知およびアプリ内メッセージを作成する前に
exl-id: c7e24338-387b-4c6f-bb29-7f7e6a1a7de5
feature: Mobile Marketing
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 80%

---

# プッシュ通知およびアプリ内メッセージを作成する前に {#before-you-create-push-notifications-and-in-app-messages}

プッシュ通知やアプリ内メッセージの作成は容易ですが、開始する前にすべてを準備する必要があります。 Marketo 管理者およびモバイルアプリデベロッパーは、必要な統合を準備するために、以下の手順に従う必要があります。

1. まず、Marketo 管理者が[モバイルアプリを追加](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md)します。

1. Marketo 管理者が[コードスニペットをデベロッパーに送信](/help/marketo/product-docs/mobile-marketing/admin/send-sdk-code-to-a-developer.md)します。

1. デベロッパーが、SDK をダウンロードし、[Android](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android) または [iOS](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-ios) 用のスニペットと他のメソッドを含めます。

1. デフォルトでは、アプリを開いたときにアプリ内メッセージがトリガーされます。 特定のページが表示されたり、特定のボタンが押されたりした場合など、他のイベントに関するメッセージをトリガーするには、デベロッパーがカスタムイベントをコードに追加する必要があります（[アプリ内メッセージのカスタムイベント](#CustomEvents)を参照）。

1. デベロッパーは、[Server API キーとプロジェクト番号](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)（Android）または[証明書とパスワード](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios)（iOS）を生成し、Marketo 管理者に送信します。

1. Marketo 管理者が [Server API キー（Android）](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-android-push-access.md) または[証明書（iOS）](/help/marketo/product-docs/mobile-marketing/admin/configure-mobile-app-ios-push-access.md)を使用してプッシュ通知アクセスを設定します。

>[!TIP]
>
>Marketo管理者は、プッシュ設定が検証されているかどうかを簡単に確認できます。 [こちら](/help/marketo/product-docs/mobile-marketing/admin/verify-push-configuration.md)にアクセスしてください。

## アプリ内メッセージのカスタムイベント {#custom-events-for-in-app-messages}

アプリ内メッセージの場合、デフォルトの表示トリガーは&#x200B;**[!UICONTROL アプリを開く]**&#x200B;に設定されています。 任意のカスタムイベントを使用してアプリ内メッセージの表示をトリガー化する場合（例：**買い物かごに追加をクリック**、**設定ページを表示**）、目的のイベントのリストを作成し、モバイルアプリデベロッパーに提供します。 次に、デベロッパーはカスタムイベントをコードに追加します。 承認されると、オーディエンスの設定時に表示トリガーとして表示されます。 **注意**：カスタムイベントコーディングの承認プロセスの完了には、時間がかかる場合があります。

アプリ内メッセージとプッシュ通知の準備をすべて終えたら、いよいよ始めましょう。

>[!MORELIKETHIS]
>
>* [アプリ内メッセージの作成](/help/marketo/product-docs/mobile-marketing/in-app-messages/creating-in-app-messages/create-an-in-app-message.md)
>
>* [プッシュ通知の作成](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)
