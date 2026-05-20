---
description: Sales Connectの購読解除メッセージの自動追加設定について説明します。 セールスメールに登録解除リンクを自動的に追加します。
title: 登録解除メッセージの自動追加設定
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
TQID: https://experienceleague.adobe.com/vF4DuUUB10XpQoMJYGquk8yptjT-5lFcMqYJB9QF7A0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 212
ht-degree: 9%

---

# 登録解除メッセージの自動追加設定 {#auto-append-unsubscribe-message-setting}

送信するすべてのメールに登録解除メッセージが含まれていることを確認し、受信者がコミュニケーションをオプトアウトするための簡単なオプションを用意します。 「購読解除メッセージを追加」が有効になっている場合、Marketo Salesから送信するすべてのコミュニケーションには、web アプリケーション、Salesforce、Gmail プラグイン、Outlook プラグインから送信されたメールを含む購読解除メッセージが含まれます。

## 注意事項 {#things-to-note}

* プラグインから送信されたメールの場合、配信停止は、テンプレートが使用されたときにのみ追加されます。

* メールテンプレートで`{{team_unsubscribe}}`動的フィールドを使用し、購読解除メッセージの追加設定が有効になっている場合、購読解除メッセージを追加する&#x200B;_ではなく、購読解除メッセージ_&#x200B;がチームの購読解除の動的フィールドに入力されます。

## 購読解除の追加を有効/無効にする {#enable-disable-unsubscribe-append}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 管理者設定で、**登録解除**&#x200B;をクリックします。

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 「メッセージ」タブの「購読解除メッセージを追加」で、スライダーを目的の状態に移動します。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>「購読解除メッセージを追加」設定を無効にした場合は、購読解除フッターをテンプレートに追加して、コミュニケーションにオプトアウトオプションがあることを確認することをお勧めします。 これは、各テンプレートに独自のカスタムメッセージを追加するか、`{{team_unsubscribe}}` [動的フィールド &#x200B;](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}を使用することで実行できます。
