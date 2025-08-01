---
description: 自動追加登録解除メッセージ設定 – Marketo ドキュメント – 製品ドキュメント
title: 登録解除メッセージの自動追加設定
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 9%

---

# 登録解除メッセージの自動追加設定 {#auto-append-unsubscribe-message-setting}

送信されたすべてのメールに購読解除メッセージが含まれていることを確認して、受信者が通信を簡単にオプトアウトできるようにします。 購読解除メッセージを追加が有効になっている場合、Marketo Sales から送信されるすべてのコミュニケーションには、Web アプリケーション、Salesforce、Gmail プラグイン、Outlook プラグインから送信されるメールを含む、購読解除メッセージが含まれます。

## 注意事項 {#things-to-note}

* プラグインから送信されるメールの場合、登録解除はテンプレートが使用される場合にのみ付加されます。

* メールテンプレートで `{{team_unsubscribe}}` 動的フィールドを使用し、購読解除メッセージの追加設定が有効になっている場合、チームの購読解除動的フィールドに、購読解除メッセージが _代わりに_ 追加されます。

## 購読解除追加を有効/無効にする {#enable-disable-unsubscribe-append}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. [ 管理設定 ] で、[**登録解除**] をクリックします。

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 「メッセージ」タブの「追加登録解除メッセージ」で、スライダーを目的の状態に移動します。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>「登録解除メッセージを追加」設定を無効にした場合、通信にオプトアウトオプションが含まれるように、テンプレートに登録解除フッターを追加することをお勧めします。 これを行うには、各テンプレートに独自のカスタムメッセージを追加するか、`{{team_unsubscribe}}` [ 動的フィールド ](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"} を使用します。
