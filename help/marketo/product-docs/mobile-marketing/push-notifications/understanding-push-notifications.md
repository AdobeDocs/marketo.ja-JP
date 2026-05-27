---
unique-page-id: 7511518
description: Marketoのプッシュ通知の詳細。 管理者と開発者の設定を理解し、スマートキャンペーンを介して作成、設定、送信します。
title: プッシュ通知について
exl-id: a3e99eeb-3671-40c4-82ac-773c2cc05914
feature: Mobile Marketing
TQID: https://experienceleague.adobe.com/PmrSIaAhfPFh0bkVdGMSKWSi9gys7z1LhLZCfpewrT4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 232
ht-degree: 80%

---

# プッシュ通知について {#understanding-push-notifications}

>[!NOTE]
>
>アプリ内メッセージは、アドオンアプリケーションです。 Marketoのアカウントマネージャーに確認して、アクティベートされていることを確認します。

Marketo モバイルエンゲージメントを使用すると、メールの作成と同様に、通知を作成、設定、送信できます。  モバイルアプリ用のプッシュ通知を作成して送信する前に、Marketo 管理者とモバイルアプリデベロッパーが設定をおこなう必要があります。

>[!CAUTION]
>
>プッシュ通知はアドオンで、開始する前に Marketo 管理者が有効にする必要があります。

## 手順 1：管理者および開発者による初期設定の実行 {#step-admin-and-developer-perform-initial-setups}

Marketo Admin とモバイルアプリの開発者が連携して設定をおこないます。 詳しくは、[プッシュ通知およびアプリ内メッセージを作成する前に](/help/marketo/product-docs/mobile-marketing/admin/before-you-create-push-notifications-and-in-app-messages.md)を参照してください。

## 手順 2：プッシュ通知を作成する {#step-create-a-push-notification}

[&#x200B; メッセージを作成](/help/marketo/product-docs/mobile-marketing/push-notifications/create-a-push-notification.md)し、AndroidおよびiOS デバイスでのメッセージの表示方法をプレビューします。

## 手順 3：送信する {#step-send}

トリガーおよびバッチスマートキャンペーンの使用して[プッシュ通知を送信できます](/help/marketo/product-docs/mobile-marketing/push-notifications/send-a-mobile-push-notification.md)。 簡単ですね。

![](assets/image2015-4-27-8-3a41-3a43.png)

>[!NOTE]
>
>* アプリが少なくとも 1 回開かれるまで、プッシュ通知は画面に表示されません。
>* iOS アプリの場合、プッシュメッセージを受信するように指定されたアプリケーションが開いていてアクティブな場合、プッシュ通知は画面に表示されません。 代わりに、アプリのローカル通知領域にメッセージが表示されます。
