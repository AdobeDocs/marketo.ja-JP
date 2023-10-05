---
description: トランザクションセールスメールテンプレート — Marketoドキュメント — 製品ドキュメント
title: トランザクションセールスメールテンプレート
feature: Sales Insight Actions
exl-id: 0178155e-f01c-449f-b510-40adf718e177
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 3%

---

# トランザクションセールスメールテンプレート {#transactional-sales-email-templates}

チームがトランザクションメールまたは非商用メールを送信する場合、メールテンプレートを非商用としてマークして、配信停止を回避できます。

## 注意事項 {#things-to-note}

* 非商用メールは、セールス配信停止および [Marketo Engage配信停止の確認](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md){target="_blank"}, but will not bypass [blocked domains](/help/marketo/product-docs/marketo-sales-insight/actions/admin/blocked-domains.md){target="_blank"}.

* 配信停止メッセージは、商用以外のメールに対して [配信停止メッセージの追加の管理者設定](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/auto-append-unsubscribe-message-setting.md){target="_blank"} is enabled. However, the `{{team_unsubscribe}}` [dynamic field](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"} チーム配信停止メッセージが引き続き表示されます。

## 非商用で使用するための電子メールテンプレートの設定 {#configure-an-email-template-for-non-commercial-use}

1. ヘッダーで、 **テンプレート**.

   ![](assets/transactional-sales-email-templates-1.png)

1. 更新するテンプレートを選択します。

   ![](assets/transactional-sales-email-templates-2.png)

1. 「テンプレート設定」で、非商用電子メールの切り替えを有効にします。

   ![](assets/transactional-sales-email-templates-3.png)

## 非商用メールの送信 {#send-a-non-commercial-email}

>[!NOTE]
>
>配信停止済みの担当者を選択すると、オレンジ色でハイライト表示されます。

1. ヘッダーで、 **作成**. 目的の非商用テンプレートを検索して選択します。

   ![](assets/transactional-sales-email-templates-4.png)

1. 非商用の E メールテンプレートを選択したことを示すバナーが表示されます。

   ![](assets/transactional-sales-email-templates-5.png)

1. 「**送信**」をクリックします。

   ![](assets/transactional-sales-email-templates-6.png)

ユーザーが購読を解除しても、E メールは送信されます。
