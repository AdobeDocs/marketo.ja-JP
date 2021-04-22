---
unique-page-id: 4719314
description: デフォルトのSalesforceフィールドマッピング —Marketoドキュメント — 製品ドキュメント
title: デフォルトのSalesforceフィールドマッピング
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 57%

---

# デフォルトのSalesforceフィールドマッピング{#default-salesforce-field-mapping}

MarketoアカウントをSalesforceと最初に同期すると、Marketoは組み込みのSalesforceフィールドとMarketoフィールドの間でこれらの関連付けを自動的に行います。 また、Marketoは、リード、アカウント、オポチュニティ、連絡先のカスタムフィールドも同期します。

## リードフィールド {#lead-fields}

| SFDCフィールド | Marketo場 |
|---|---|
| 年間収益 | 年間収益 |
| 都市 | 都市 |
| 企業 | 企業名 |
| 変換日 | SFDC 変換日 |
| 国 | 国 |
| 作成日 | SFDC 作成日 |
| 詳細 | 担当者の注記 |
| メール | メールアドレス |
| ファックス | ファックス番号 |
| 名  | 名  |
| メールオプトアウト | 配信停止完了 |
| 業界 | 業界 |
| コンバート済み | SFDC 変換済み |
| 削除済み | SFDC 削除済み |
| 姓 | 姓 |
| リード ソース | ソース |
| リードスコア | スコア |
| 携帯電話番号 | 携帯電話番号 |
| 従業員 | 従業員数 |
| 電話 | 電話番号 |
| 郵便番号 | 郵便番号 |
| 評価 | 評価 |
| 敬称 | 敬称 |
| 都道府県 | 都道府県 |
| ステータス | ステータス |
| 所在地住所 | 住所 |
| 件名 | 職位 |
| ウェブサイト | ウェブサイト |

## 取引先責任者フィールド {#contact-fields}

| SFDCフィールド | Marketo場 |
|---|---|
| 生年月日 | 生年月日 |
| 作成日 | SFDC 作成日 |
| 連絡先の説明 | 担当者の注記 |
| メール | メールアドレス |
| 勤務先FAX | ファックス番号 |
| 名  | 名  |
| メールオプトアウト | 配信停止完了 |
| 削除済み | SFDC 削除済み |
| 姓 | 姓 |
| リード ソース | ソース |
| リードスコア | スコア |
| MailingCity | 都市 |
| MailingCountry | 国 |
| MailingPostalCode | 郵便番号 |
| MailingState | 都道府県 |
| MailingStreet | 住所 |
| 携帯電話番号 | 携帯電話番号 |
| 業務用電話番号 | 電話番号 |
| 敬称 | 敬称 |
| 件名 | 職位 |

## アカウントフィールド {#account-fields}

| SFDCフィールド | Marketo場 |
|---|---|
| 年間収益 | 年間収益 |
| 請求先住所 (都市) | 請求先住所 (都市) |
| 請求先住所 (国) | 請求先住所 (国) |
| 請求先の郵便番号 | 請求先住所 (郵便番号) |
| 請求先の州/郡 | 請求先住所 (都道府県) |
| 請求先 | 請求先住所 |
| アカウントの説明 | 企業注記 |
| 業界 | 業界 |
| 削除済み | SFDC 削除済み |
| アカウント名 | 企業名 |
| 従業員 | 従業員数 |
| アカウントの電話番号 | 代表電話番号 |
| SIC コード | SIC コード |
| アカウントサイト | サイト |
| アカウントタイプ | SFDC のタイプ |
| ウェブサイト | ウェブサイト |

## MarketoのSalesforce関連システムフィールド（読み取り専用） {#salesforce-related-system-fields-in-marketo-read-only}

これらのフィールドはMarketoで作成されますが、顧客は調整できません。

| フィールド | 詳細 |
|---|---|
| SFDC ID | 18文字のSalesforce Id |
| SFDC のタイプ | リードまたは連絡先。 リードが空の場合、リードはMarketoの個人としてのみ存在します |
| SFDC 作成日 | SFDCで作成された日付(Marketoで作成された日付とは異なる場合があります) |
| SFDCが削除されました | SFDCにいた人が削除され、現在はMarketoにしか住んでいない |
