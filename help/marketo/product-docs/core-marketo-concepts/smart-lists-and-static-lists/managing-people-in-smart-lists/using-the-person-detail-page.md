---
unique-page-id: 2953415
description: 個人の詳細ページの使用 —Marketoドキュメント — 製品ドキュメント
title: 「個人詳細」ページの使用
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 50%

---

# 個人の詳細ページの使用{#using-the-person-detail-page}

人物詳細ページには、Marketoが人物について知っているすべての情報が含まれています。 このページからデータを直接編集できます。

## 個人の詳細ページへのアクセス{#getting-to-person-detail-page}

特定の人を開く方法はたくさんあります。 次に例を示します。

* **データベース**&#x200B;から、クイック検索で検索できます
* 任意のスマート&#x200B;**リスト**&#x200B;またはリスト
* **プログラム** のメンバー
* **表示キャンペーン** メンバーシンアスマートキャンペーン
* **レポート**の一部

   <br> 

1. 任意の人を重複クリックするか、左側のIDをシングルクリックします。

   ![](assets/one-1.png)

1. これで、個人の詳細画面が開きます。

   ![](assets/two-5.png)

## ページ構成 — Salesforce {#page-organization-salesforce}

個人情報は、次のタブに分類されます。

| タブ | 詳細 |
|---|---|
| 情報 | 連絡先情報およびユーザー設定のフィールド。 |
| 企業情報 | 個人の会社情報と住所。 |
| 商談情報 | Salesforceから同期されたオポチュニティ情報。 |
| SFDC リードフィールド | 組み込みのSalesforceフィールド。 |
| SFDCカスタムフィールド | カスタムのSalesforceフィールド。 |
| アクティビティログ | その人に関連するすべてのアクティビティ。 |

## ページ構成 — Microsoft Dynamics {#page-organization-microsoft-dynamics}

| タブ | 詳細 |
|---|---|
| 情報 | 連絡先情報およびユーザー設定のフィールド。 |
| 企業情報 | 個人の会社情報と住所。 |
| 商談情報 | Microsoftから同期されたオポチュニティ情報。 |
| Microsoft カスタムフィールド | ユーザー設定のMicrosoftフィールド |
| Microsoft リードフィールド | 組み込みのMicrosoftフィールド |
| アクティビティログ | その人に関連するすべてのアクティビティ。 |

>[!NOTE]
>
>また、CRMと同期されていないインスタンスのオポチュニティ情報[がAPI](http://developers.marketo.com/rest-api/lead-database/opportunities/)から挿入されていることも確認できます。

## フィールドの編集{#editing-a-field}

編集可能なフィールドが多数あります。 ユーザーの情報を更新するには、新しい値を入力し、フィールドの外側をクリックして保存します。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM同期前のMarketoの既定のフィールド{#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| 住所 | 年間収益 | 匿名 IP | 請求先住所 | 請求先住所 (都市) |
| 請求先住所 (国) | 請求先住所 (郵便番号) | 請求先住所 (都道府県) | 都市 | 企業名 |
| 国 | 作成時刻 | 生年月日 | 部門 | 連絡拒否 |
| 電話連絡拒否の原因 | 電話連絡拒否の理由 | メールアドレス | メール無効 | メール無効の理由 |
| 外部企業ID | 外部セールス担当者ID | ファックス番号 | 名 | 氏名 |
| 業界 | 推測される都市 | 推測される企業 | 推測される国 | 推測される都市圏 |
| 推測される市外局番 | 推測される郵便番号 | 推測される都道府県/地域 | 匿名 | 顧客 |
| パートナー | 役職 | 姓 | 評価 | スコア |
| リードソース | ステータス | 代表電話番号 | Marketo ソーシャル Facebook の表示名 | Marketo ソーシャル Facebook ID |
| Marketo ソーシャル Facebook の画像 URL | Marketo ソーシャル Facebook のプロファイル URL | Marketo ソーシャル Facebook のリーチ | Marketo ソーシャル Facebook を参照元とする登録数 | Marketo ソーシャル Facebook を参照元とする訪問数 |
| Marketo ソーシャルジェンダ | Marketo ソーシャルを最後の参照元とする登録 | Marketo ソーシャルを最後の参照元とする訪問 | Marketo ソーシャル LinkedIn の表示名 | Marketo ソーシャル LinkedIn Id |
| Marketo ソーシャル LinkedIn の画像 URL | Marketo ソーシャル LinkedIn のプロファイル URL | Marketo ソーシャル LinkedIn のリーチ | Marketo ソーシャル LinkedIn を参照元とする登録数 | Marketo ソーシャル LinkedIn を参照元とする訪問数 |
| Marketo ソーシャル Syndication ID | Marketo ソーシャルを参照元とする合計登録数 | Marketo ソーシャルを参照元とする合計訪問数 | Marketo ソーシャル Twitter の表示名 | Marketo ソーシャル Twitter Id |
| Marketo ソーシャル Twitter の画像 URL | Marketo ソーシャル Twitter のプロファイル URL | Marketo ソーシャル Twitter のリーチ | Marketo ソーシャル Twitter を参照元とする登録数 | Marketo ソーシャル Twitter を参照元とする訪問数 |
| ミドルネーム | 携帯電話番号 | 従業員数 | 電話番号 | 郵便番号 |
| 優先順位 | 相対スコア | ロール | 敬称 | SIC コード |
| サイト | 都道府県 | 配信停止完了 | 配信停止の理由 | 更新時刻 |
| 緊急度 | ウェブサイト |  |  |  |

>[!NOTE]
>
>一部のフィールドは編集できません&#x200B;__:
>
>* アクティビティログ
>* 会社情報
>* SFDCの連絡先のオポチュニティ
>* 「作成日」や「元のソースの種類」など、Marketo固有のフィールドがあります。

>
>
[システム管理フィールド](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md)の詳細を表示します。

>[!MORELIKETHIS]
>
>[個人の詳細ページ用のカスタムタブの作成](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
