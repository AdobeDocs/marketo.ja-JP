---
description: Sales Connectのトランザクションセールスメールテンプレートについて説明します。 トランザクションメッセージの登録解除をバイパスするテンプレートを使用します。
title: トランザクションセールスメールテンプレート
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 6%

---

# トランザクションセールスメールテンプレート {#transactional-sales-email-templates}

取引メールや非商用メールを送信する場合、メールテンプレートを非商用メールとしてマークすることで、配信停止を回避できます。

## 注意事項 {#things-to-note}

* 非商用メールは、セールスの登録解除と[Marketo Engageの登録解除チェック &#x200B;](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}をバイパスしますが、[&#x200B; ブロックされたドメイン &#x200B;](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"}はバイパスされません。

* 購読解除メッセージの追加管理設定[&#128279;](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"}が有効になっている場合でも、購読解除メッセージは非商用メールに自動的に追加されません。 ただし、`{{team_unsubscribe}}` [動的フィールド &#x200B;](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}は、引き続きチームの購読解除メッセージに入力されます。

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
