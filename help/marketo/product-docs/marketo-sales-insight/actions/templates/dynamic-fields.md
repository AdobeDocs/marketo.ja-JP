---
description: 動的フィールド — Marketoドキュメント — 製品ドキュメント
title: 動的フィールド
hide: true
hidefromtoc: true
source-git-commit: a0b10255513c13b7100b667513e3e61fc3788a15
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 78%

---

# 動的フィールド {#dynamic-fields}

メールテンプレートを、`{{first_name}}` や `{{company}}` のような事前定義済みの属性を使用してパーソナライズできます。これらのフィールドを使用すると、複数の連絡先にメールを送信したり、これらのフィールドを連絡先ごとに個別に入力する必要なしに自動入力したりできます。

>[!TIP]
>
>「first_name」および「company」フィールドは、Sales Insight Actions と Salesforce の両方に表示される唯一のフィールドです。 つまり、連絡先が [web アプリケーション](https://toutapp.com/login)に存在しない場合、Salesforce が調べられ、一致するメールアドレスを持つ連絡先／リードレコードが見つかるかどうかが確認されます。その後、そのレコードの情報を使用してフィールドにデータを入力します。

## テンプレートへの動的フィールドの挿入 {#insert-a-dynamic-field-into-a-template}

1. **テンプレートとキャンペーン**&#x200B;で、編集するテンプレートを見つけて、「**テンプレートを編集**」をクリックします。

1. クリック **ダイナミックフィールドの挿入**.

   >[!NOTE]
   >
   >Sales Insight アクションに存在する連絡先を電子メールで送信する場合は、基本的な動的フィールドを使用できます。 これらは、連絡先から直接引き出されます。

Salesforce に存在する連絡先にメールを送信する場合は、Salesforce の動的フィールドを利用できます。これらはすべて「sfdc」で始まります。Salesforce に連携している限り、これらのフィールドでは Salesforce 内のリード／連絡先が直接呼び出され、テンプレートに情報が入力されます。

## 件名行に動的フィールドを挿入 {#insert-dynamic-fields-in-a-subject-line}

メールの件名フィールドに手動でコピーペーストするだけで、適切な形式になっていることを確認できます。

## 動的フィールド用語集 {#dynamic-fields-glossary}

Sales Insight アクションでテンプレートを作成する場合は、 **ダイナミックフィールドの挿入** 」ボタンをクリックします。

このツールは、`auto-personalize your email` に使用されて `pulling information from the People page` によって時間を大幅に節約できます。

| 動的フィールド | メールに表示される内容の例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith さん |
| `{{friendly_unsubscribe}}` | 再度通知を受けたくない場合は、こちらからお知らせください |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | https://www.marketo.com |

**注意事項**：

* 連絡先の情報が正しく入力されていない場合やリードページに表示されていない場合は、テンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の連絡先の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、連絡先の詳細では必ず、Inc.または Co.をコンマで区切ってください。Sales Insight のアクションは、値を取り込む際に何を削除するかを知っています。
* メールテンプレートを、`{{my_name}}` や `{{my_title}}` のような事前定義済みの属性を使用してパーソナライズできます。これらのフィールドを使用すると、メールテンプレートですばやく自己参照できます。

>[!TIP]
>
>ダイナミックフィールドに値が入力されない場合は、 [この記事](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
