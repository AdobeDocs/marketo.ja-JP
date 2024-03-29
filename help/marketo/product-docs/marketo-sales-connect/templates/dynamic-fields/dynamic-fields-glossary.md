---
unique-page-id: 14352509
description: 動的フィールド用語集 — Marketo ドキュメント — 製品ドキュメント
title: 動的フィールド用語集
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: cffe7a8734f79f887f3aad017a16fad4f04cda74
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 63%

---

# 動的フィールド用語集 {#dynamic-fields-glossary}

Sales Connect でテンプレートを作成する場合は、動的フィールドを統合し、「**MSE 動的フィールド**」ボタンをクリックします。

このツールは、`auto-personalize your email` に使用されて `pulling information from the People page` によって時間を大幅に節約できます。

| 動的フィールド | メールに表示される内容の例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith さん |
| `{{team_unsubscribe}}` | 今後メールの受信を希望しない場合は、ここをクリックしてください |
| `{{friendly_unsubscribe}}` | メールに飽きた？ こちらにお知らせください |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | シニアテクニカルライター、Keith Flynn -Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | https://www.adobe.com |

**注意事項**：

* 取引先責任者の情報が正しく入力されていない場合や人物ページに表示されていない場合は、情報がテンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の取引先責任者の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、連絡先の詳細では必ず、Inc.または Co.をコンマで区切ってください。これは、Sales Connect が、値を取り込む際に削除する必要があるものを認識する方法です。
* システムは、送信される各電子メールにユーザーの署名を自動的に追加します。 ユーザーが `{{my_signature}}` 動的フィールドの場合、システムは署名を入力します。 `{{my_signature}}` 動的フィールドが配置されました。 重複を避けるために、ここにのみ追加されます。 システムが処理します `{{team_unsubscribe}}` グローバルな append unsubscribe 設定が有効な場合も同様です。

>[!TIP]
>
>メールに自動的に取り込みたいものについては、独自の[カスタム動的フィールド](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)を作成できます。
