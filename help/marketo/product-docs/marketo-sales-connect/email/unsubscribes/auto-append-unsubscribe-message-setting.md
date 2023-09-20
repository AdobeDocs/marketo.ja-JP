---
description: 自動追加配信停止メッセージ設定 — Marketoドキュメント — 製品ドキュメント
title: 配信停止メッセージの自動追加設定
hide: true
hidefromtoc: true
feature: Marketo Sales Connect
source-git-commit: b0f62abfe04efd8e72ed8e92442d4a46ea118f33
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 5%

---

# 配信停止メッセージの自動追加設定 {#auto-append-unsubscribe-message-setting}

送信されるすべての E メールに配信停止メッセージが含まれていることを確認して、受信者が簡単に通信をオプトアウトできるようにします。 配信停止メッセージの追加を有効にすると、チームがMarketo Sales から送信するすべての通信に、配信停止メッセージ（Web アプリケーション、Salesforce、Gmail プラグイン、Outlook プラグインから送信されたメールを含む）が含まれます。

## 注意事項 {#things-to-note}

* プラグインから送信された E メールの場合、配信停止は、テンプレートが使用された場合にのみ追加されます。

* を使用する場合、 `{{team_unsubscribe}}` e メールテンプレートの「動的」フィールドで、「配信停止メッセージの追加」設定が有効になっている場合、チーム配信停止の動的フィールドに配信停止メッセージが入力されます _の代わりに_ 配信停止メッセージを追加する

## 配信停止の追加を有効/無効にする {#enable-disable-unsubscribe-append}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 「管理者設定」で、 **配信停止**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 「メッセージング」タブの「配信停止メッセージを追加」で、スライダーを目的の状態に移動します。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>配信停止メッセージの追加設定を無効にした場合、テンプレートに配信停止フッターを追加して、通信にオプトアウトオプションが設定されていることを確認することをお勧めします。 これをおこなうには、独自のカスタムメッセージを各テンプレートに追加するか、 `{{team_unsubscribe}}` 動的フィールド。
