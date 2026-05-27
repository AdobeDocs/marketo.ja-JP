---
description: 取引用セールスメールテンプレートと、登録解除リンクが必要ない場合について説明します。 1対1のトランザクションメッセージに使用します。
title: トランザクションセールスメールテンプレート
feature: Sales Insight Actions
exl-id: 0178155e-f01c-449f-b510-40adf718e177
TQID: https://experienceleague.adobe.com/jtFUKYM-28npTije11gtCPNGBdsgEcI6Qhp6lbbLWUY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 194
ht-degree: 6%

---

# トランザクションセールスメールテンプレート {#transactional-sales-email-templates}

取引メールや非商用メールを送信する場合、メールテンプレートを非商用メールとしてマークすることで、配信停止を回避できます。

## 注意事項 {#things-to-note}

* 非商用メールは、セールスの登録解除と[Marketo Engageの登録解除チェック ](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}をバイパスしますが、[ ブロックされたドメイン ](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}はバイパスされません。

* 購読解除メッセージの追加管理設定](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"}が有効になっている場合でも、購読解除メッセージは非商用メールに自動的に追加されません。 [ただし、`{{team_unsubscribe}}` [動的フィールド ](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}は、引き続きチームの購読解除メッセージに入力されます。

## 非商用利用のためのメールテンプレートの設定 {#configure-an-email-template-for-non-commercial-use}

1. ヘッダーで、**テンプレート**&#x200B;をクリックします。

   ![](assets/transactional-sales-email-templates-1.png)

1. 更新するテンプレートを検索して選択します。

   ![](assets/transactional-sales-email-templates-2.png)

1. テンプレート設定で非商用メールトグルを有効にします。

   ![](assets/transactional-sales-email-templates-3.png)

## 商用以外の電子メールの送信 {#send-a-non-commercial-email}

>[!NOTE]
>
>購読解除したユーザーを選択すると、オレンジ色で強調表示されます。

1. ヘッダーで、**作成**&#x200B;をクリックします。 目的の非商用テンプレートを検索して選択します。

   ![](assets/transactional-sales-email-templates-4.png)

1. ユーザーは、非商用メールテンプレートを選択したことを示すバナーを見ることができます。

   ![](assets/transactional-sales-email-templates-5.png)

1. 「**送信**」をクリックします。

   ![](assets/transactional-sales-email-templates-6.png)

登録解除しても、メールは送信されます。
