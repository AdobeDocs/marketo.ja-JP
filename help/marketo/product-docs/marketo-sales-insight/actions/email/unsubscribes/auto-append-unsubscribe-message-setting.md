---
description: セールスメールの自動追加登録解除メッセージを有効または無効にする方法について説明します。
title: 登録解除メッセージの自動追加設定
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
TQID: https://experienceleague.adobe.com/4iAq0-giVwuDcqaoi8QnLN35QO67RSlgHYXFYaUebZg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 184
ht-degree: 9%

---

# 登録解除メッセージの自動追加設定 {#auto-append-unsubscribe-message-setting}

送信するすべてのSales Insight Actions メールに登録解除メッセージが含まれていることを確認し、受信者がコミュニケーションをオプトアウトする簡単なオプションを用意します。 「購読解除メッセージを追加」が有効になっている場合、Marketo Salesから送信するすべてのコミュニケーションには、web アプリケーションとSalesforceから送信されたメールを含む購読解除メッセージが含まれます。

>[!NOTE]
>
>メールテンプレートで`{{team_unsubscribe}}`動的フィールドを使用し、購読解除メッセージの追加設定が有効になっている場合、購読解除メッセージを追加する&#x200B;_ではなく、購読解除メッセージ_&#x200B;がチームの購読解除の動的フィールドに入力されます。

## 購読解除の追加を有効/無効にする {#enable-disable-unsubscribe-append}

1. 歯車アイコンをクリックし、「**設定**」を選択します。

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. 管理者設定で、**登録解除**&#x200B;をクリックします。

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. 「メッセージ」タブの「購読解除メッセージを追加」で、スライダーを目的の状態に移動します。

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>「購読解除メッセージを追加」設定を無効にした場合は、購読解除フッターをテンプレートに追加して、コミュニケーションにオプトアウトオプションがあることを確認することをお勧めします。 これは、各テンプレートに独自のカスタムメッセージを追加するか、`{{team_unsubscribe}}` [動的フィールド ](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}を使用することで実行できます。
