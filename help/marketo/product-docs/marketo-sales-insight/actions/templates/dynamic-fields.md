---
description: 動的フィールド - Marketo ドキュメント - 製品ドキュメント
title: 動的フィールド
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 100%

---

# 動的フィールド {#dynamic-fields}

メールテンプレートを、`{{first_name}}` や `{{company}}` のような事前定義済みの属性を使用してパーソナライズできます。動的フィールドを使用すると、複数の取引先責任者にメールを送信したり、フィールドを取引先責任者ごとに入力せずに自動入力したりできます。

>[!TIP]
>
>「名前（名）」フィールドと「会社」フィールドは、Sales Insight Actions と Salesforce の両方に表示される唯一のフィールドです。つまり、取引先責任者が [web アプリケーション](https://toutapp.com/login)に存在しない場合、Salesforce を調べて、一致するメールアドレスを持つ取引先責任者／リードレコードが見つかるかどうかを確認します。その後、そのレコードの情報を使用してフィールドにデータを入力します。

## テンプレートへの動的フィールドの挿入 {#insert-a-dynamic-field-into-a-template}

1. **テンプレートとキャンペーン**&#x200B;で、編集するテンプレートを見つけて、「**テンプレートを編集**」をクリックします。

1. 「**動的フィールドを挿入**」をクリックします。

   >[!NOTE]
   >
   >Sales Insight Actions に存在する取引先責任者にメールを送信する場合は、基本的な動的フィールドを使用できます。それらのフィールドは、取引先責任者から直接引き出されます。

Salesforce に存在する取引先責任者にメールを送信する場合は、Salesforce の動的フィールドを利用できます。フィールドはすべて「sfdc」で始まります。Salesforce と連携している限り、動的フィールドは Salesforce 内のリード／取引先責任者を直接呼び出し、テンプレートに情報を入力します。

## 件名行に動的フィールドを挿入 {#insert-dynamic-fields-in-a-subject-line}

メールの件名フィールドに手動でコピーペーストするだけで、適切な形式になっていることを確認できます。

## 動的フィールド用語集 {#dynamic-fields-glossary}

Sales Insight Actions でテンプレートを作成する場合は、必ず「**動的フィールドを挿入**」ボタンをクリックして動的フィールドを統合することを推奨します。

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

* 取引先責任者の情報が正しく入力されていない場合や人物ページに表示されていない場合は、情報がテンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の取引先責任者の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、取引先責任者の詳細では必ず、Inc. または Co. をコンマで区切ってください。これにより、Sales Insight Actions が値を取り込む際に削除する必要があるものを認識します。
* メールテンプレートを、`{{my_name}}` や `{{my_title}}` のような事前定義済みの属性を使用してパーソナライズできます。これらのフィールドを使用すると、メールテンプレートですばやく自己参照できます。

>[!TIP]
>
>動的フィールドに値が入力されない場合は、[この記事](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md)を参照してください。
