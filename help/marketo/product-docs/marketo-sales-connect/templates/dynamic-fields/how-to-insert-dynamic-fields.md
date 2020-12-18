---
unique-page-id: 14352592
description: 動的フィールドの挿入方法 — Marketto Docs — 製品ドキュメント
title: 動的フィールドの挿入方法
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# 動的フィールドの挿入方法{#how-to-insert-dynamic-fields}

Eメールテンプレートを、`{{first_name}}`や`{{company}}`などの定義済みの属性でパーソナライズできます。 これらのフィールドを使用すると、複数の連絡先を電子メールで送信し、これらのフィールドに個別に入力する必要なく、自動入力できます。

>[!TIP]
>
>「first_name」と「会社」フィールドは`only fields that will look to both Sales Connect and Salesforce.`です。つまり、[Webアプリ](http://toutapp.com/login)に連絡先が存在しない場合、Salesforceで、一致する電子メールアドレスを持つ連絡先/リードレコードが見つかるかどうかを確認します。 その後、そのレコードの情報を使用してフィールドに入力します。

## テンプレートへの動的フィールドの挿入{#insert-a-dynamic-field-into-a-template}

1. **テンプレートとキャンペーン**&#x200B;で、編集するテンプレートを探し、「**テンプレートを編集**」をクリックします。
1. 「**動的フィールドをトゥー**」をクリックします。

   >[!NOTE]
   >
   >Sales Connectに存在する連絡先を電子メールで送信する場合は、基本的な動的フィールドを使用できます。 これらは、連絡先から直接引っ張られます。

Salesforceに存在する連絡先を電子メールで送信する場合は、Salesforce動的フィールドを利用できます。 これらはすべて「sfdc」で始まります。 Salesforceに接続している限り、これらのフィールドはSalesforceのリード/連絡先に直接呼び出され、テンプレートに情報が入力されます。

## 件名行に動的フィールドを挿入{#insert-dynamic-fields-in-a-subject-line}

電子メールの件名フィールドに手動でコピー&amp;ペーストするだけで、正しい形式が保たれていることを確認できます。
