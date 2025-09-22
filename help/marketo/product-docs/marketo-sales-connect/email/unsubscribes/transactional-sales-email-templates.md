---
description: トランザクション販売のメールテンプレート - Marketo ドキュメント – 製品ドキュメント
title: トランザクションセールスメールテンプレート
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 7%

---

# トランザクションセールスメールテンプレート {#transactional-sales-email-templates}

チームがトランザクションメールまたは非商用メールを送信している場合、メールテンプレートを非商用としてマークすると、購読解除をバイパスできます。

## 注意事項 {#things-to-note}

* 非商用メールは、販売の購読解除および [Marketo Engageの購読解除チェック ](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"} をバイパスしますが、[ ブロックされたドメイン ](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md){target="_blank"} はバイパスしません。

* [ 登録解除メッセージを追加する管理設定 ](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} が有効になっている場合でも、非商用メールに登録解除メッセージが自動的に追加されることはありません。 ただし、`{{team_unsubscribe}}` [ 動的フィールド ](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"} は、引き続きチームの購読解除メッセージに入力されます。

## 非商用で使用するためのメールテンプレートの設定 {#configure-an-email-template-for-non-commercial-use}

1. ヘッダーで、「**テンプレート**」をクリックします。

   ![](assets/transactional-sales-email-templates-1.png)

1. 更新するテンプレートを検索して選択します。

   ![](assets/transactional-sales-email-templates-2.png)

1. テンプレート設定の非商用メール切り替えスイッチを有効にします。

   ![](assets/transactional-sales-email-templates-3.png)

## 非商用メールの送信 {#send-a-non-commercial-email}

>[!NOTE]
>
>登録解除したユーザーが選択されると、オレンジ色でハイライト表示されます。

1. ヘッダーで、「作成 **をクリックし** す。 目的の非商用テンプレートを検索して選択します。

   ![](assets/transactional-sales-email-templates-4.png)

1. 非商用のメールテンプレートを選択したことを示すバナーが表示されます。

   ![](assets/transactional-sales-email-templates-5.png)

1. 「**送信**」をクリックします。

   ![](assets/transactional-sales-email-templates-6.png)

購読を解除した場合でも、メールは送信されます。
