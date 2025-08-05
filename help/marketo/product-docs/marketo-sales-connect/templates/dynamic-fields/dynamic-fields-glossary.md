---
unique-page-id: 14352509
description: 動的フィールド用語集 — Marketo ドキュメント — 製品ドキュメント
title: 動的フィールド用語集
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 56%

---

# 動的フィールド用語集 {#dynamic-fields-glossary}

[!DNL Sales Connect] でテンプレートを作成する場合は、常に「**[!UICONTROL MSE 動的フィールド]** ボタンを使用して動的フィールドを統合することをお勧めします。

このツールは、`auto-personalize your email` に使用されて `pulling information from the [!UICONTROL People] page` によって時間を大幅に節約できます。

| 動的フィールド | メールに表示される内容の例 |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith さん |
| `{{team_unsubscribe}}` | 私たちからのメールの受信を希望しない場合は、ここをクリックしてください |
| `{{friendly_unsubscribe}}` | メールにはうんざりですか？ こちらにお知らせください |
| `{{my_name}}` | キース・フリン |
| `{{my_signature}}` | Keith Flynn （シニアテクニカルライター） – Adobe |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | シニアテクニカルライター |
| `{{work_website}}` | <https://www.adobe.com> |

**注意事項**：

* 取引先責任者の情報が正しく入力されていない場合や人物ページに表示されていない場合は、情報がテンプレートに正しく取り込まれません。
* `{{company}}` と `{{company_friendly}}` の違いは、`{{company_friendly}}` では顧客の取引先責任者の会社名から Inc.、LLC.などの正式な名称が削除されることです。
* `{{company_friendly}}` を使用する場合、連絡先の詳細では必ず、Inc.または Co.をコンマで区切ってください。これは、Sales Connect が、値を取り込む際に削除する必要があるものを認識する方法です。
* システムは、送信される各メールにユーザーの署名を自動的に追加します。 ユーザーが `{{my_signature}}` 動的フィールドを含むテンプレートを使用している場合、システムは、`{{my_signature}}` 動的フィールドが配置されている署名を入力します。 重複を避けるために追加されたものだけです。 グローバル `{{team_unsubscribe}}` 追加購読解除設定が有効になっている場合、システムは同じように処理します。

>[!TIP]
>
>メールに自動的に取り込みたいものについては、独自の[カスタム動的フィールド](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md)を作成できます。
