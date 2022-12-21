---
unique-page-id: 4719314
description: デフォルトの Salesforce フィールドマッピング — Marketo ドキュメント — 製品ドキュメント
title: デフォルトの Salesforce フィールドマッピング
exl-id: d6639733-f85d-4f4c-ac41-5d2a68a9c6b2
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 100%

---

# デフォルトの Salesforce フィールドマッピング {#default-salesforce-field-mapping}

Marketo アカウントと Salesforce の初回同期時に、Marketo では組み込みの Salesforce フィールドと Marketo フィールドの間でこれらの関連付けが自動的におこなわれます。リード、アカウント、商談、連絡先のカスタムフィールドも同期されます。

## リードフィールド {#lead-fields}

| SFDC フィールド | Marketo フィールド |
|---|---|
| 年間売上高 | 年間売上高 |
| 市区町村 | 市区町村 |
| 企業 | 企業名 |
| コンバージョン日 | SFDC 変換日 |
| 国 | 国 |
| 作成日 | SFDC 作成日 |
| 説明 | 顧客の注記 |
| メール | メールアドレス |
| FAX | FAX 番号 |
| 名 | 名 |
| メールオプトアウト | 登録解除済み |
| 業界 | 業界 |
| コンバージョン済み | SFDC コンバージョン済み |
| 削除済み | SFDC 削除済み |
| 姓 | 姓 |
| リードのソース | ソース |
| リードのスコア | スコア |
| 携帯電話 | 携帯電話番号 |
| 従業員 | 従業員数 |
| 電話 | 電話番号 |
| 郵便番号 | 郵便番号 |
| 評価 | 評価 |
| 敬称 | 敬称 |
| 都道府県 | 都道府県 |
| ステータス | ステータス |
| 番地 | 住所 |
| 職位 | 職位 |
| Web サイト | Web サイト |

## 連絡先フィールド {#contact-fields}

| SFDC フィールド | Marketo フィールド |
|---|---|
| 生年月日 | 生年月日 |
| 作成日 | SFDC 作成日 |
| 連絡先の説明 | 顧客の注記 |
| メール | メールアドレス |
| 勤務先 FAX | FAX 番号 |
| 名 | 名 |
| メールオプトアウト | 登録解除済み |
| 削除済み | SFDC 削除済み |
| 姓 | 姓 |
| リードのソース | ソース |
| リードのスコア | スコア |
| MailingCity | 市区町村 |
| MailingCountry | 国 |
| MailingPostalCode | 郵便番号 |
| MailingState | 都道府県 |
| MailingStreet | 住所 |
| 携帯電話 | 携帯電話番号 |
| 勤務先電話 | 電話番号 |
| 敬称 | 敬称 |
| 職位 | 職位 |

## アカウントフィールド {#account-fields}

| SFDC フィールド | Marketo フィールド |
|---|---|
| 年間売上高 | 年間売上高 |
| 請求先住所 (市区町村) | 請求先住所 (市区町村) |
| 請求先住所 (国) | 請求先住所 (国) |
| 請求先住所 (郵便番号) | 請求先住所 (郵便番号) |
| 請求先住所 (都道府県） | 請求先住所 (都道府県) |
| 請求先住所（番地） | 請求先住所 |
| アカウントの説明 | 企業注記 |
| 業界 | 業界 |
| 削除済み | SFDC 削除済み |
| アカウント名 | 企業名 |
| 従業員 | 従業員数 |
| アカウントの電話 | 代表電話 |
| SIC コード | SIC コード |
| アカウントサイト | サイト |
| アカウントタイプ | SFDC のタイプ |
| Web サイト | Web サイト |

## Marketo の Salesforce 関連システムフィールド（読み取り専用） {#salesforce-related-system-fields-in-marketo-read-only}

これらのフィールドは Marketo で作成されますが、顧客は調整できません。

| フィールド | 説明 |
|---|---|
| SFDC ID | 18 文字の Salesforce ID |
| SFDC のタイプ | リードまたは連絡先。空の場合、リードは Marketo にのみ存在します |
| SFDC 作成日 | SFDC で作成された日付（Marketo で作成された日付とは異なる場合があります） |
| SFDC 削除済み | 以前は SFDC に存在したが、削除され、現在は Marketo にしか存在しない個人 |
