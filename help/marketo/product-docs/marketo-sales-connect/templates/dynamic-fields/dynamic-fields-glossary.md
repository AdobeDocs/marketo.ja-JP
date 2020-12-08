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


# 動的フィールドの用語集 {#dynamic-fields-glossary}

Sales Connectでテンプレートを作成する場合は、「 **MSE Dynamic Fields** 」ボタンを使用して、動的フィールドを統合することを常にお勧めします。

このツールは、までに多くの時間 `auto-personalize your email` を節約するために使用され `pulling information from the People page`ます。

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

* 連絡先がユーザーページに表示され `information is entered incorrectly` ていないか、表示されていない場合は、その連絡先がテンプレート `will not pull over correctly` に表示されます。

* との違い `{{company}}` は、Inc.、LLC `{{company_friendly}}``{{company_friendly}}``remove any formal title`など、お客様の担当者の会社の名前からの意志との違いです。
* を使用する場合 `{{company_friendly}}`は、Inc.またはCo.をコンマで区切って連絡先の詳細を入力してください。 Sales Connectは、値を取り込む際に何を取り除くかを次のように認識します。

>[!TIP]
>
>電子メールに自動的に取り込む必要のある任意の [カスタム動的フィールドを独自に作成できます](http://docs.marketo.com/x/fADb) 。

