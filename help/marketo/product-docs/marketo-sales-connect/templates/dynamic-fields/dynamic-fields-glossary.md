---
unique-page-id: 14352509
description: 動的フィールド用語集 — Marketo ドキュメント — 製品ドキュメント
title: 動的フィールド用語集
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: d6a3d95ed42d1c08d69014e1aa013e7436bd06c2
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 97%

---

# 動的フィールド用語集 {#dynamic-fields-glossary}

Sales Connect でテンプレートを作成する場合は、動的フィールドを統合し、「**MSE 動的フィールド**」ボタンをクリックします。

このツールは、`auto-personalize your email` に使用されて `pulling information from the People page` によって時間を大幅に節約できます。

| 動的フィールド | メールに表示される内容の例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith さん |
| `{{friendly_unsubscribe}}` | 再度通知を受けたくない場合は、こちらからお知らせください |
| `{{my_name}}` | Keith Flynn |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | https://www.adobe.com |

**注意事項**：

* 取引先責任者の情報が正しく入力されていない場合や人物ページに表示されていない場合は、情報がテンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の取引先責任者の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、連絡先の詳細では必ず、Inc.または Co.をコンマで区切ってください。これは、Sales Connect が、値を取り込む際に削除する必要があるものを認識する方法です。

>[!TIP]
>
>メールに自動的に取り込みたいものについては、独自の[カスタム動的フィールド](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)を作成できます。
