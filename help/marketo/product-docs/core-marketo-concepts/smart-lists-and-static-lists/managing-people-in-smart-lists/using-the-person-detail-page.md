---
unique-page-id: 2953415
description: 人物の詳細ページの使用 - Marketo ドキュメント - 製品ドキュメント
title: 人物の詳細ページの使用
exl-id: 8476ed02-6d94-4aa5-91f6-55c81a87f745
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 85%

---

# 人物の詳細ページの使用 {#using-the-person-detail-page}

人物の詳細ページには、ある人物に関して Marketo に記録されているすべての情報が表示されます。このページから直接、データを編集することができます。

## 人物の詳細ページへのアクセス {#getting-to-person-detail-page}

特定の人物を開く方法は多数あります。以下に例を示します。

* **データベース**&#x200B;から、「クイック検索」で検索できます
* 任意の&#x200B;**スマートリスト**&#x200B;またはリスト
* プログラムの「**メンバー**」タブ
* **スマートキャンペーン**&#x200B;内のキャンペーンメンバーの表示
* **レポート**
  <br> 

1. 任意の人物をダブルクリックするか、左側の ID をシングルクリックします。

   ![](assets/one-1.png)

1. 人物の詳細画面が表示されます。

   ![](assets/two-5.png)

## ページ組織 - Salesforce {#page-organization-salesforce}

人物情報は以下のタブに分類されています。

| タブ | 説明 |
|---|---|
| 情報 | 人物に関する取引先責任者情報およびカスタムフィールド。 |
| 企業情報 | 人物の企業情報と住所。 |
| 商談情報 | Salesforce から同期される商談情報。 |
| SFDC リードフィールド | ビルトインの Salesforce のフィールド。 |
| SFDC カスタムフィールド | Salesforce のカスタムフィールド。 |
| アクティビティログ | 人物に関連するすべてのアクティビティ。 |

## ページ組織 - Microsoft Dynamics {#page-organization-microsoft-dynamics}

| タブ | 説明 |
|---|---|
| 情報 | 人物に関する取引先責任者情報およびカスタムフィールド。 |
| 企業情報 | 人物の企業情報と住所。 |
| 商談情報 | マイクロソフトから同期される商談情報。 |
| マイクロソフトカスタムフィールド | マイクロソフトのカスタムフィールド。 |
| マイクロソフトリードフィールド | ビルトインの Microsoft のフィールド。 |
| アクティビティログ | 人物に関連するすべてのアクティビティ。 |

>[!NOTE]
>
>CRM と同期されていないインスタンスの商談情報が [API を介して挿入](https://experienceleague.adobe.com/ja/docs/marketo-developer/marketo/rest/lead-database/opportunities)されていることも確認できます。

## フィールドの編集 {#editing-a-field}

多くのフィールドは編集可能です。人物の情報を更新するには、新しい値を入力し、フィールドの外側をクリックして保存します。

![](assets/image2015-2-27-11-3a14-3a2.png)

## CRM 同期前の Marketo のデフォルトフィールド {#marketo-default-fields-prior-to-crm-sync}

|   |  |  |  |  |
|---|---|---|---|---|
| 住所 | 年間収益 | 匿名 IP | 請求先住所 | 請求先住所（市区町村） |
| 請求先住所（国） | 請求先住所（郵便番号） | 請求先住所（都道府県） | 市区町村 | 企業名 |
| 国 | 作成日時 | 生年月日 | 部門 | 電話連絡拒否 |
| 電話連絡拒否の原因 | 電話連絡拒否の理由 | メールアドレス | メール無効 | メール無効の理由 |
| 外部企業 ID | 外部セールス担当者 ID | ファックス番号 | 名 | 氏名 |
| 業界 | 推測される市区町村 | 推測される企業 | 推測される国 | 推測される都市圏 |
| 推測される市外局番 | 推測される郵便番号 | 推測される都道府県／地域 | 匿名 | 顧客 |
| パートナー | 役職 | 姓 | 評価 | スコア |
| 人物のソース | ステータス | 代表電話番号 | Marketo Social [!DNL Facebook] の表示名 | Marketo Social [!DNL Facebook] Id |
| Marketo Social [!DNL Facebook] の写真 URL | Marketo Social [!DNL Facebook] プロファイル URL | Marketo Social [!DNL Facebook] Reach | Marketo Social [!DNL Facebook] の参照登録 | Marketo Social [!DNL Facebook] 関連の訪問 |
| Marketo ソーシャル性別 | Marketo ソーシャルを最後の参照元とする登録 | Marketo ソーシャルを最後の参照元とする訪問 | Marketo Social [!DNL LinkedIn] の表示名 | Marketo Social [!DNL LinkedIn] Id |
| Marketo Social [!DNL LinkedIn] の写真 URL | Marketo Social [!DNL LinkedIn] プロファイル URL | Marketo Social [!DNL LinkedIn] Reach | Marketo Social [!DNL LinkedIn] の参照登録 | Marketo Social [!DNL LinkedIn] 関連の訪問 |
| Marketo ソーシャル Syndication ID | Marketo ソーシャルを参照元とする合計登録数 | Marketo ソーシャルを参照元とする合計訪問数 | Marketo Social [!DNL Twitter] の表示名 | Marketo Social [!DNL Twitter] Id |
| Marketo Social [!DNL Twitter] の写真 URL | Marketo Social [!DNL Twitter] プロファイル URL | Marketo Social [!DNL Twitter] Reach | Marketo Social [!DNL Twitter] の参照登録 | Marketo Social [!DNL Twitter] 関連の訪問 |
| ミドルネーム | 携帯電話番号 | 従業員数 | 電話番号 | 郵便番号 |
| 優先度 | 相対スコア | ロール | 敬称 | SIC コード |
| サイト | ステート | 登録解除 | 登録解除の理由 | 更新時刻 |
| 緊急度 | Web サイト |  |  |  |

>[!NOTE]
>
>一部のフィールドは&#x200B;_編集不可_&#x200B;です。
>
>* アクティビティログ
>* 会社情報
>* SFDC 取引先責任者の商談
>* 作成日や元のソースタイプなど、Marketo 固有の特定のフィールド。
>
>詳細は[システム管理フィールド](/help/marketo/product-docs/administration/field-management/understanding-system-managed-fields.md){target="_blank"}をご覧ください。

>[!MORELIKETHIS]
>
>[人物の詳細ページ用のカスタムタブの作成](/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md){target="_blank"}
