---
unique-page-id: 14352592
description: 動的フィールドの挿入方法 — Marketo ドキュメント — 製品ドキュメント
title: 動的フィールドの挿入方法
exl-id: e4989350-872d-47a1-84b0-210e631ae23a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 100%

---

# 動的フィールドの挿入方法 {#how-to-insert-dynamic-fields}

メールテンプレートを、`{{first_name}}` や `{{company}}` のような事前定義済みの属性を使用してパーソナライズできます。これらのフィールドを使用すると、複数の連絡先にメールを送信したり、これらのフィールドを連絡先ごとに個別に入力する必要なしに自動入力したりできます。

>[!TIP]
>
>「first_name」フィールドと「company」フィールドは、Sales Connect と Salesforce の両方に表示される唯一のフィールドです。つまり、連絡先が [web アプリケーション](https://toutapp.com/login)に存在しない場合、Salesforce が調べられ、一致するメールアドレスを持つ連絡先／リードレコードが見つかるかどうかが確認されます。その後、そのレコードの情報を使用してフィールドにデータを入力します。

## テンプレートへの動的フィールドの挿入 {#insert-a-dynamic-field-into-a-template}

1. **テンプレートとキャンペーン**&#x200B;で、編集するテンプレートを見つけて、「**テンプレートを編集**」をクリックします。

1. 「**Tout の動的フィールド**」をクリックします。

   >[!NOTE]
   >
   >Sales Connect に存在する連絡先にメールを送信する場合は、基本的な動的フィールドを使用できます。これらは、連絡先から直接引き出されます。

Salesforce に存在する取引先責任者にメールを送信する場合は、Salesforce の動的フィールドを利用できます。フィールドはすべて「sfdc」で始まります。Salesforce と連携している限り、動的フィールドは Salesforce 内のリード／取引先責任者を直接呼び出し、テンプレートに情報を入力します。

## 件名行に動的フィールドを挿入 {#insert-dynamic-fields-in-a-subject-line}

メールの件名フィールドに手動でコピーペーストするだけで、適切な形式になっていることを確認できます。
