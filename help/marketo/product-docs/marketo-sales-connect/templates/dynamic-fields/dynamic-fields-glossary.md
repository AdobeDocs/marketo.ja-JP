---
unique-page-id: 14352509
description: 動的フィールド用語集 — Marketto Docs — 製品ドキュメント
title: 動的フィールドの用語集
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# 動的フィールド用語集{#dynamic-fields-glossary}

Sales Connectでテンプレートを作成する場合は、**MSE動的フィールド**&#x200B;ボタンを使用して、動的フィールドを統合することを常にお勧めします。

このツールは`auto-personalize your email`に使われ、`pulling information from the People page`までに時間を節約できます。

| 動的フィールド | 電子メールに表示する内容の例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | キース |
| `{{friendly_unsubscribe}}` | もし私からの連絡が来たくないのなら、こちらにお知らせください |
| `{{my_name}}` | アラン・ブラドリー |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | https://www.marketo.com |

**注意事項**:

* 連絡先の情報が正しく入力されていないか、[人]ページに表示されていない場合は、正しくテンプレートに引き継がれません。
* `{{company}}`と`{{company_friendly}}`の違いは、`{{company_friendly}}`は、お客様の連絡先の会社の名前から、Inc.、LLC.などの正式なタイトルを削除することです。
* `{{company_friendly}}`を使用する場合は、Inc.またはCo.をコンマで区切って連絡先の詳細を入力してください。 Sales Connectは、値を取り込む際に何を取り除くかを次のように認識します。

>[!TIP]
>
>電子メールに自動的に取り込む必要のある任意のユーザーに対して、独自の[カスタム動的フィールド](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)を作成できます
