---
unique-page-id: 14352509
description: 動的フィールド用語集 — Marketo ドキュメント — 製品ドキュメント
title: 動的フィールド用語集
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 100%

---

# 動的フィールド用語集 {#dynamic-fields-glossary}

[!DNL Sales Connect] でテンプレートを作成する場合は、「**[!UICONTROL MSE 動的フィールド]**」ボタンを使用して、動的フィールドを統合することを常にお勧めします。

このツールは、`auto-personalize your email` に使用されて `pulling information from the [!UICONTROL People] page` によって時間を大幅に節約できます。

| 動的フィールド | メールに表示される内容の例 |
|---|---|
| `{{company}}` | アドビ |
| `{{company_friendly}}` | アドビ |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | 今後当社からのメールの受信を希望しない場合は、こちらをクリックしてください |
| `{{friendly_unsubscribe}}` | メールにうんざりしていませんか？こちらからお知らせください |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn、シニアテクニカルライター - アドビ |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | <https://www.adobe.com> |

**注意事項**：

* 取引先責任者の情報が正しく入力されていない場合や人物ページに表示されていない場合は、情報がテンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の取引先責任者の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、連絡先の詳細では必ず、Inc.または Co.をコンマで区切ってください。これは、Sales Connect が、値を取り込む際に削除する必要があるものを認識する方法です。
* システムにより、送信される各メールにユーザの署名が自動的に追加されます。ユーザが `{{my_signature}}` 動的フィールドを含むテンプレートを使用している場合、`{{my_signature}}` 動的フィールドが配置されている場所に署名が入力されます。重複を避けるために、署名はその場所にのみ追加されます。グローバル追加登録解除設定が有効になっている場合、システムにより `{{team_unsubscribe}}` も同様に処理されます。

>[!TIP]
>
>メールに自動的に取り込むものについては、独自の[カスタム動的フィールド](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)を作成できます。
