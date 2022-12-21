---
unique-page-id: 7511518
description: プッシュ通知について - Marketo ドキュメント - 製品ドキュメント
title: プッシュ通知について
exl-id: a3e99eeb-3671-40c4-82ac-773c2cc05914
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 100%

---

# プッシュ通知について {#understanding-push-notifications}

>[!NOTE]
>
>アプリ内メッセージは、アドオンアプリケーションです。Marketo のアカウントマネージャーに問い合わせて、アクティベートされていることを確認します。

Marketo モバイルエンゲージメントを使用すると、メールの作成と同様に、通知を作成、設定、送信できます。モバイルアプリ用のプッシュ通知を作成して送信する前に、Marketo 管理者とモバイルアプリデベロッパーが設定をおこなう必要があります。

>[!CAUTION]
>
>プッシュ通知はアドオンで、開始する前に Marketo 管理者が有効にする必要があります。

## 手順 1：管理者および開発者による初期設定の実行 {#step-admin-and-developer-perform-initial-setups}

Marketo Admin とモバイルアプリの開発者が連携して設定をおこないます。詳しくは、[プッシュ通知およびアプリ内メッセージを作成する前に](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md)を参照してください。

## 手順 2：プッシュ通知を作成する {#step-create-a-push-notification}

[メッセージを作成](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)して Android および iOS デバイスでの表示をプレビューできます。

## 手順 3：送信する {#step-send}

トリガーおよびバッチスマートキャンペーンの使用して[プッシュ通知を送信できます](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)。簡単ですね。

![](assets/image2015-4-27-8-3a41-3a43.png)

>[!NOTE]
>
>* アプリが少なくとも 1 回開かれるまで、プッシュ通知は画面に表示されません。
>* iOS アプリの場合、プッシュメッセージを受信するように指定されたアプリケーションが開いていてアクティブな場合、プッシュ通知は画面に表示されません。代わりに、アプリのローカル通知領域にメッセージが表示されます。

