---
unique-page-id: 2953415
description: リードの詳細ページの使用 - Marketo ドキュメント - 製品ドキュメント
title: リードの詳細ページの使用
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '550'
ht-degree: 100%

---

# リードの詳細ページの使用 {#using-the-person-detail-page}

リードの詳細ページには、あるリードに関して Marketo に記録されているすべての情報が表示されます。このページから直接、データを編集することができます。

## リードの詳細ページへのアクセス {#getting-to-person-detail-page}

特定のリードを開く方法は多数あります。以下に例を示します。

* **データベース**&#x200B;から、「クイック検索」で検索できます
* 任意のスマート&#x200B;**リスト**&#x200B;またはリスト
* プログラムの「**メンバー**」タブ
* **スマートキャンペーン**&#x200B;内のキャンペーンメンバーの表示
* **レポート**

   <br>

1. 任意のリードをダブルクリックするか、左側の ID をシングルクリックします。

   ![](assets/one-1.png)

1. リードの詳細画面が表示されます。

   ![](assets/two-5.png)

## ページ組織 - Salesforce {#page-organization-salesforce}

リード情報は以下のタブに分類されています。

| タブ | 説明 |
|---|---|
| 情報 | リードに関する連絡先情報およびカスタムフィールド。 |
| 企業情報 | リードの企業情報と住所。 |
| 商談情報 | Salesforce から同期される商談情報。 |
| SFDC リードフィールド | 組み込み済みの Salesforce のフィールド。 |
| SFDC カスタムフィールド | Salesforce のカスタムフィールド。 |
| アクティビティログ | リードに関連するすべてのアクティビティ。 |

## ページ組織 - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| タブ | 説明 |
|---|---|
| 情報 | リードに関する連絡先情報およびカスタムフィールド。 |
| 企業情報 | リードの企業情報と住所。 |
| 商談情報 | マイクロソフトから同期される商談情報。 |
| マイクロソフトカスタムフィールド | マイクロソフトのカスタムフィールド。 |
| マイクロソフトリードフィールド | 組み込み済みのマイクロソフトのフィールド。 |
| アクティビティログ | リードに関連するすべてのアクティビティ。 |

>[!NOTE]
>
>CRM と同期されていないインスタンスの商談情報が [API を介して挿入](http://developers.marketo.com/rest-api/lead-database/opportunities/)されていることも確認できます。

## フィールドの編集 {#editing-a-field}

多くのフィールドは編集可能です。リードの情報を更新するには、新しい値を入力し、フィールドの外側をクリックして保存します。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM 同期前の Marketo のデフォルトフィールド {#marketo-default-fields-prior-to-crm-sync}

|  |  |  |  |  |
|---|---|---|---|---|
| 住所 | 年間売上高 | 匿名 IP | 請求先住所 | 請求先住所（都市） |
| 請求先住所（国） | 請求先住所（郵便番号） | 請求先住所（都道府県） | 都市 | 企業名 |
| 国 | 作成日時 | 生年月日 | 部門 | 電話連絡拒否 |
| 電話連絡拒否の原因 | 電話連絡拒否の理由 | メールアドレス | メール無効 | メール無効の理由 |
| 外部企業 ID | 外部セールス担当者 ID | ファックス番号 | 名 | 氏名 |
| 業界 | 推測される都市 | 推測される企業 | 推測される国 | 推測される都市圏 |
| 推測される市外局番 | 推測される郵便番号 | 推測される都道府県／地域 | 匿名 | 顧客 |
| パートナー | 職位 | 姓 | 評価 | スコア |
| リードソース | ステータス | 代表電話番号 | Marketo ソーシャル Facebook の表示名 | Marketo ソーシャル Facebook ID |
| Marketo ソーシャル Facebook の画像 URL | Marketo ソーシャル Facebook のプロファイル URL | Marketo ソーシャル Facebook のリーチ | Marketo ソーシャル Facebook を参照元とする登録数 | Marketo ソーシャル Facebook を参照元とする訪問数 |
| Marketo ソーシャル性別 | Marketo ソーシャルを最後の参照元とする登録 | Marketo ソーシャルを最後の参照元とする訪問 | Marketo ソーシャル LinkedIn の表示名 | Marketo ソーシャル LinkedIn Id |
| Marketo ソーシャル LinkedIn の画像 URL | Marketo ソーシャル LinkedIn のプロファイル URL | Marketo ソーシャル LinkedIn のリーチ | Marketo ソーシャル LinkedIn を参照元とする登録数 | Marketo ソーシャル LinkedIn を参照元とする訪問数 |
| Marketo ソーシャル Syndication ID | Marketo ソーシャルを参照元とする合計登録数 | Marketo ソーシャルを参照元とする合計訪問数 | Marketo ソーシャル Twitter の表示名 | Marketo ソーシャル Twitter Id |
| Marketo ソーシャル Twitter の画像 URL | Marketo ソーシャル Twitter のプロファイル URL | Marketo ソーシャル Twitter のリーチ | Marketo ソーシャル Twitter を参照元とする登録数 | Marketo ソーシャル Twitter を参照元とする訪問数 |
| ミドルネーム | 携帯電話番号 | 従業員数 | 電話番号 | 郵便番号 |
| 優先順位 | 相対スコア | ロール | 敬称 | SIC コード |
| サイト | ステート | 登録解除 | 登録解除の理由 | 更新時刻 |
| 緊急度 | Web サイト |  |  |  |

>[!NOTE]
>
>一部のフィールドは&#x200B;_編集不可_&#x200B;です。
>
>* アクティビティログ
>* 会社情報
>* SFDC 連絡先の商談
>* 作成日や元のソースタイプなど、Marketo 固有の特定のフィールド。

>
>詳細は[システム管理フィールド](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md)をご覧ください。

>[!MORELIKETHIS]
>
>[ユーザーの詳細ページ用のカスタムタブの作成](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md)
