---
description: 動的フィールド - Marketo ドキュメント - 製品ドキュメント
title: 動的フィールド
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 60%

---

# 動的フィールド {#dynamic-fields}

メールテンプレートを、`{{first_name}}` や `{{company}}` のような事前定義済みの属性を使用してパーソナライズできます。動的フィールドを使用すると、複数の取引先責任者にメールを送信したり、フィールドを取引先責任者ごとに入力せずに自動入力したりできます。

>[!TIP]
>
>「first_name」フィールドと「company」フィールドは、[!DNL Sales Insight Actions] と [!DNL Salesforce] の両方に参照される唯一のフィールドです。 つまり、[web アプリケーション ](https://toutapp.com/login) に連絡先が存在しない場合は、一致するメールアドレスを持つ連絡先/ リードレコードが見つかるかどうかを [!DNL Salesforce] で確認します。 その後、そのレコードの情報を使用してフィールドにデータを入力します。

## テンプレートへの動的フィールドの挿入 {#insert-a-dynamic-field-into-a-template}

1. **[!UICONTROL テンプレートとキャンペーン]**&#x200B;で、編集するテンプレートを見つけて、「**[!UICONTROL テンプレートを編集]**」をクリックします。

1. 「**[!UICONTROL 動的フィールドを挿入]**」をクリックします。

   >[!NOTE]
   >
   >[!DNL Sales Insight Actions] に存在する連絡先にメールを送信する際に、基本的な動的フィールドを使用できます。 それらのフィールドは、取引先責任者から直接引き出されます。

[!DNL Salesforce] に存在する連絡先にメールを送信する場合は、[!DNL Salesforce] の動的フィールドを利用できます。 フィールドはすべて「sfdc」で始まります。[!DNL Salesforce] への接続がある限り、これらのフィールドはテンプレートに情報を入力するた [!DNL Salesforce] にリード/連絡先を直接呼び出します。

## 件名行に動的フィールドを挿入 {#insert-dynamic-fields-in-a-subject-line}

メールの件名フィールドに手動でコピーペーストするだけで、適切な形式になっていることを確認できます。

## ダイナミックフィールドのデフォルト値 {#dynamic-field-default-values}

メールテンプレートにダイナミックフィールドを追加する際に、使用できる値がない場合、ダイナミックフィールドが解決するデフォルト値を追加できます。

これを行うには、ダイナミックフィールドラベルの後に &quot;|&quot; を追加してから、&quot;default:&quot; を追加します（共に引用符は含めない）。次に、値が見つからない場合にフィールドで解決させる値を追加します（引用符で囲む）。

**例：**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## 動的フィールド用語集 {#dynamic-fields-glossary}

[!DNL Sales Insight Actions] でテンプレートを作成する場合は、常に「**[!UICONTROL 動的フィールドを挿入]** ボタンを使用して動的フィールドを統合することをお勧めします。

このツールは、`auto-personalize your email` に使用されて `pulling information from the People page` によって時間を大幅に節約できます。

| 動的フィールド | メールに表示される内容の例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith さん |
| `{{team_unsubscribe}}` | 私たちからのメールの受信を希望しない場合は、ここをクリックしてください |
| `{{friendly_unsubscribe}}` | メールにはうんざりですか？ こちらにお知らせください |
| `{{my_name}}` | キース・フリン |
| `{{my_signature}}` | Keith Flynn （シニアテクニカルライター） – Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | https://www.adobe.com |

**注意事項**：

* 取引先責任者の情報が正しく入力されていない場合や人物ページに表示されていない場合は、情報がテンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の取引先責任者の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、取引先責任者の詳細では必ず、Inc. または Co. をコンマで区切ってください。値を取り込む際に削除 [!DNL Sales Insight Actions] る内容を把握するには、次の方法があります。
* メールテンプレートを、`{{my_name}}` や `{{my_title}}` のような事前定義済みの属性を使用してパーソナライズできます。これらのフィールドを使用すると、メールテンプレートですばやく自己参照できます。
* システムは、送信される各メールにユーザーの署名を自動的に追加します。 ユーザーが `{{my_signature}}` 動的フィールドを含むテンプレートを使用している場合、システムは、`{{my_signature}}` 動的フィールドが配置されている署名を入力します。 重複を避けるために追加されたものだけです。 グローバル `{{team_unsubscribe}}` 追加購読解除設定が有効になっている場合、システムは同じように処理します。

>[!TIP]
>
>動的フィールドに値が入力されない場合は、[この記事](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md)を参照してください。
