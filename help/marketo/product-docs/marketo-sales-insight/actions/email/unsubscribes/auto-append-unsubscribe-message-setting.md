---
description: 自動追加配信停止メッセージ設定 — Marketoドキュメント — 製品ドキュメント
title: 配信停止メッセージの自動追加設定
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 4%

---

# 配信停止メッセージの自動追加設定 {#auto-append-unsubscribe-message-setting}

送信されたすべての Sales Insight Actions メールに配信停止メッセージが含まれていることを確認して、受信者が簡単に通信をオプトアウトできるようにします。 「配信停止メッセージを追加」が有効な場合、チームがMarketo Sales から送信するすべての通信には、Web アプリケーションや Salesforce から送信されたメールを含む配信停止メッセージが含まれます。

>[!NOTE]
>
>を使用する場合、 `{{team_unsubscribe}}` e メールテンプレートの「動的」フィールドで、「配信停止メッセージの追加」設定が有効になっている場合、チーム配信停止の動的フィールドに配信停止メッセージが入力されます _の代わりに_ 配信停止メッセージを追加する

## 配信停止の追加を有効/無効にする {#enable-disable-unsubscribe-append}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 「管理者設定」で、 **配信停止**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 「メッセージング」タブの「配信停止メッセージを追加」で、スライダーを目的の状態に移動します。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>配信停止メッセージの追加設定を無効にした場合、テンプレートに配信停止フッターを追加して、通信にオプトアウトオプションが設定されていることを確認することをお勧めします。 これをおこなうには、独自のカスタムメッセージを各テンプレートに追加するか、 `{{team_unsubscribe}}` [動的フィールド](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
