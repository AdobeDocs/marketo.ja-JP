---
unique-page-id: 4719314
description: デフォルトのSalesforceフィールドマッピング — Marketto Docs — 製品ドキュメント
title: デフォルトのSalesforceフィールドマッピング
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# デフォルトのSalesforceフィールドマッピング{#default-salesforce-field-mapping}

MarketoのアカウントをSalesforceと最初に同期すると、Marketoは組み込みのSalesforceフィールドとMarketoフィールドの間でこれらの関連付けを自動的に行います。 また、マーケティング担当者は、リード、アカウント、オポチュニティ、連絡先のカスタムフィールドも同期します。

## リードフィールド{#lead-fields}

| SFDCフィールド | Marketoフィールド |
|---|---|
| 年間売上高 | 年間売上高 |
| 市区町村 | 市区町村 |
| 会社 | 会社名 |
| 変換日 | SFDC変換日 |
| 国 | 国 |
| 作成日 | SFDCの作成日 |
| 説明 | 個人メモ |
| 電子メール | 電子メールアドレス |
| FAX | Fax番号 |
| 名 | 名 |
| 電子メオプトアウトール | 登録解除 |
| 業界 | 業界 |
| 変換済み | SFDCが変換される |
| 削除済み | SFDCが削除されました |
| 姓 | 姓 |
| リードソース | ソース |
| リードスコア | スコア |
| 携帯電話 | 携帯電話番号 |
| 従業員 | 従業員数 |
| 電話 | 電話番号 |
| 郵便番号 | 郵便番号 |
| 評価 | 評価 |
| 挨拶 | 挨拶 |
| 都道府県 | 州 |
| ステータス | ステータス |
| 通り | 住所 |
| タイトル | 肩書 |
| Webサイト | Webサイト |

## 連絡先フィールド{#contact-fields}

| SFDCフィールド | Marketoフィールド |
|---|---|
| 誕生日 | 生年月日 |
| 作成日 | SFDCの作成日 |
| 連絡先の説明 | 個人メモ |
| 電子メール | 電子メールアドレス |
| 勤務先FAX | Fax番号 |
| 名 | 名 |
| 電子メオプトアウトール | 登録解除 |
| 削除済み | SFDCが削除されました |
| 姓 | 姓 |
| リードソース | ソース |
| リードスコア | スコア |
| MailingCity | 市区町村 |
| MailingCountry | 国 |
| MailingPostalCode | 郵便番号 |
| MailingState | 州 |
| MailingStreet | 住所 |
| 携帯電話 | 携帯電話番号 |
| 勤務先の電話 | 電話番号 |
| 挨拶 | 挨拶 |
| タイトル | 肩書 |

## アカウントフィールド{#account-fields}

| SFDCフィールド | Marketoフィールド |
|---|---|
| 年間売上高 | 年間売上高 |
| 請求先の市区町村 | 請求先の市区町村 |
| 請求国 | 請求国 |
| 請求先の郵便番号 | 請求先郵便番号 |
| 請求先の州/郡 | 請求先の州 |
| 請求先 | 請求先住所 |
| アカウントの説明 | 会社に関する注意 |
| 業界 | 業界 |
| 削除済み | SFDCが削除されました |
| アカウント名 | 会社名 |
| 従業員 | 従業員数 |
| アカウントの電話番号 | メイン電話 |
| SICコード | SICコード |
| アカウントサイト | サイト |
| アカウントタイプ | SFDCタイプ |
| Webサイト | Webサイト |

## MarketoのSalesforce関連システムフィールド（読み取り専用） {#salesforce-related-system-fields-in-marketo-read-only}

これらのフィールドはMarketoで作成されますが、顧客は調整できません。

| フィールド | 説明 |
|---|---|
| SFDC ID | 18文字のSalesforce Id |
| SFDCタイプ | リードまたは連絡先。 空の場合、リードはMarketoの担当者としてのみ存在します |
| SFDCの作成日 | SFDCで作成された日付（マーケティング担当者が作成した日付とは異なる場合があります） |
| SFDCが削除されました | 以前はSFDCにいたが削除され、現在はマーケットにのみ住んでいる |
