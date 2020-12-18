---
unique-page-id: 14352509
description: 動的フィールド用語集 — Marketto Docs — 製品ドキュメント
title: 動的フィールドの用語集
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[電子メールで保護]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | https://www.marketo.com |

**注意事項**:

* 連絡先の`information is entered incorrectly`がない場合、またはユーザーページに連絡先がない場合は、テンプレートに`will not pull over correctly`が挿入されます。

* `{{company}}`と`{{company_friendly}}`の違いは、`{{company_friendly}}`が`remove any formal title`（Inc.、LLC.など）を&lt;a2/>とし、連絡先の会社の名前から選ぶことです。
* `{{company_friendly}}`を使用する場合は、Inc.またはCo.をコンマで区切って連絡先の詳細を入力してください。 Sales Connectは、値を取り込む際に何を取り除くかを次のように認識します。

>[!TIP]
>
>電子メールに自動的に取り込む必要のある任意のユーザーに対して、独自の[カスタム動的フィールド](http://docs.marketo.com/x/fADb)を作成できます

