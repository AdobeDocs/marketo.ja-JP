---
description: 自動追加登録解除メッセージ設定 – Marketo ドキュメント – 製品ドキュメント
title: 登録解除メッセージの自動追加設定
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 8%

---

# 登録解除メッセージの自動追加設定 {#auto-append-unsubscribe-message-setting}

送信されたすべての営業インサイトアクションのメールに購読解除メッセージが含まれていることを確認して、受信者がコミュニケーションを簡単にオプトアウトできるようにします。 登録解除メッセージの追加が有効になっている場合、Marketo Sales から送信されるすべてのコミュニケーションには、Web アプリケーションや Salesforce から送信されるメールを含む、登録解除メッセージが含まれます。

>[!NOTE]
>
>メールテンプレートで `{{team_unsubscribe}}` 動的フィールドを使用し、購読解除メッセージの追加設定が有効になっている場合、チームの購読解除動的フィールドに、購読解除メッセージが _代わりに_ 追加されます。

## 購読解除追加を有効/無効にする {#enable-disable-unsubscribe-append}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. [ 管理設定 ] で、[**登録解除**] をクリックします。

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 「メッセージ」タブの「追加登録解除メッセージ」で、スライダーを目的の状態に移動します。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>「登録解除メッセージを追加」設定を無効にした場合、通信にオプトアウトオプションが含まれるように、テンプレートに登録解除フッターを追加することをお勧めします。 これを行うには、各テンプレートに独自のカスタムメッセージを追加するか、`{{team_unsubscribe}}` [ 動的フィールド ](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} を使用します。
