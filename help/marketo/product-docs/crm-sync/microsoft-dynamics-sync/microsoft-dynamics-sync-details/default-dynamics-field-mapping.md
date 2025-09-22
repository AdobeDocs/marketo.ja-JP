---
description: デフォルトの Dynamics フィールドマッピング - Marketo ドキュメント - 製品ドキュメント
title: デフォルトの Dynamics フィールドマッピング
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 100%

---

# デフォルトの Dynamics フィールドマッピング {#default-dynamics-field-mapping}

Marketo Engage アカウントを Microsoft と最初に同期すると、Marketo はビルトインの Dynamics フィールドと Marketo フィールドの間でこれらの関連付けを自動的に行います。Marketo は、リード、アカウント、商談、取引先責任者のカスタムフィールドも同期します。

## リードフィールド {#lead-fields}

<table>
  <colgroup>
    <col>
    <col>
    <col>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo フィールド</th>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft の作成日]</td>
      <td>[!UICONTROL 作成日]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL 敬称]</td>
      <td>[!UICONTROL 敬称]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL 名]</td>
      <td>[!UICONTROL 名前（名）]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL ミドルネーム]</td>
      <td>[!UICONTROL ミドルネーム]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL 姓]</td>
      <td>[!UICONTROL 名前（姓）]</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>[!UICONTROL メール]</td>
      <td>[!UICONTROL メール]</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 役職]</td>
      <td>[!UICONTROL 役職]</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>[!UICONTROL 電話]</td>
      <td>[!UICONTROL 業務用電話]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL モバイル]</td>
      <td>[!UICONTROL 携帯電話]</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>[!UICONTROL FAX]</td>
      <td>[!UICONTROL FAX]</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>[!UICONTROL アドレス]</td>
      <td>[!UICONTROL 番地 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 市区町村]</td>
      <td>[!UICONTROL 市区町村]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL 都道府県]</td>
      <td>[!UICONTROL 州／都道府県]</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>[!UICONTROL 国]</td>
      <td>[!UICONTROL 国／地域]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL 郵便番号]</td>
      <td>[!UICONTROL 郵便番号]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人ソース]</td>
      <td>[!UICONTROL リードソース]</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人ステータス]</td>
      <td>[!UICONTROL ステータス]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL ステータス理由]</td>
      <td>[!UICONTROL ステータス理由]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人の注記]</td>
      <td>[!UICONTROL 説明]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL 電話連絡拒否]</td>
      <td>[!UICONTROL 電話を許可しない]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL 登録解除済み]</td>
      <td>[!UICONTROL 一括メールを送信しない]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人評価]</td>
      <td>[!UICONTROL 評価]</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 住所 2]</td>
      <td>[!UICONTROL 番地 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 住所 3]</td>
      <td>[!UICONTROL 番地 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft メール送信除外]</td>
      <td>[!UICONTROL メールを許可しない]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft FAX送信除外]</td>
      <td>[!UICONTROL FAXを許可しない]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft マーケティング資料の受領拒否]</td>
      <td>[!UICONTROL マーケティング資料]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 自宅電話]</td>
      <td>[!UICONTROL 自宅電話]</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 希望連絡方法]</td>
      <td>[!UICONTROL 希望連絡方法]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft トピック]</td>
      <td>[!UICONTROL トピック]</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションの日付]</td>
      <td>[!UICONTROL 最新の注目のアクションの日付]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションの説明]</td>
      <td>[!UICONTROL 最新の注目のアクションの説明]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションのソース]</td>
      <td>[!UICONTROL 最新の注目のアクションのソース]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションのタイプ]</td>
      <td>[!UICONTROL 最新の注目のアクションのタイプ]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社]</td>
      <td>[!UICONTROL 会社名]</td>
      <td>companyname</td>
    </tr>
    <tr>
      <td>[!UICONTROL 相対スコア]</td>
      <td>[!UICONTROL 相対スコア]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL 優先度]</td>
      <td>[!UICONTROL 優先度]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL 相対緊急度]</td>
      <td>[!UICONTROL 緊急度]</td>
      <td>mkt_ecqurency</td>
    </tr>
    <tr>
      <td>[!UICONTROL 件名]</td>
      <td>[!UICONTROL トピック]</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>[!UICONTROL 年間収益]</td>
      <td>[!UICONTROL 年間収益]</td>
      <td>revenue</td>
    </tr>
  </tbody>
</table>

以下のリードフィールドは、内部で使用するために同期されます。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL 所有者]</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 作成日]</td>
      <td>createdon</td>
    </tr>
  </tbody>
</table>

## 取引先責任者フィールド {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo フィールド</th>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft の作成日]</td>
      <td>[!UICONTROL 作成日]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL 敬称]</td>
      <td>[!UICONTROL 敬称]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL 名]</td>
      <td>[!UICONTROL 名前（名）]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL ミドルネーム]</td>
      <td>[!UICONTROL ミドルネーム]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL 姓]</td>
      <td>[!UICONTROL 名前（姓）]</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>[!UICONTROL メール]</td>
      <td>[!UICONTROL メール]</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 役職]</td>
      <td>[!UICONTROL 役職]</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>[!UICONTROL 電話]</td>
      <td>[!UICONTROL 業務用電話]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL モバイル]</td>
      <td>[!UICONTROL 携帯電話]</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>[!UICONTROL アドレス]</td>
      <td>[!UICONTROL 住所 1：番地 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 市区町村]</td>
      <td>[!UICONTROL 住所 1：市区町村]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL 都道府県]</td>
      <td>[!UICONTROL 住所 1：州／都道府県]</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>[!UICONTROL 国]</td>
      <td>[!UICONTROL 住所 1：国／地域]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL 郵便番号]</td>
      <td>[!UICONTROL 住所 1：郵便番号]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人ステータス]</td>
      <td>[!UICONTROL ステータス]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL ステータス理由]</td>
      <td>[!UICONTROL ステータス理由]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 電話連絡拒否]</td>
      <td>[!UICONTROL 電話を許可しない]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL 登録解除済み]</td>
      <td>[!UICONTROL 一括メールを送信しない]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 住所 2]</td>
      <td>[!UICONTROL 住所 1：番地 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 住所 3]</td>
      <td>[!UICONTROL 住所 1：番地 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft メール送信除外]</td>
      <td>[!UICONTROL メールを許可しない]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 自宅電話]</td>
      <td>[!UICONTROL 自宅電話]</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 希望連絡方法]</td>
      <td>[!UICONTROL 希望連絡方法]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションの日付]</td>
      <td>[!UICONTROL 最新の注目のアクションの日付]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションのタイプ]</td>
      <td>[!UICONTROL 最新の注目のアクションのタイプ]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションのソース]</td>
      <td>[!UICONTROL 最新の注目のアクションのソース]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最新の注目のアクションの説明]</td>
      <td>[!UICONTROL 最新の注目のアクションの説明]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft マーケティング資料の受領拒否]</td>
      <td>[!UICONTROL マーケティング資料]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft FAX送信除外]</td>
      <td>[!UICONTROL Microsoft FAX送信除外]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL 優先度]</td>
      <td>[!UICONTROL 優先度]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL 相対緊急度]</td>
      <td>[!UICONTROL 緊急度]</td>
      <td>mkt_ecqurency</td>
    </tr>
    <tr>
      <td>[!UICONTROL 相対スコア]</td>
      <td>[!UICONTROL 相対スコア]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人の注記]</td>
      <td>[!UICONTROL 説明]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人スコア]</td>
      <td>[!UICONTROL リードスコア]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL 個人の注記]</td>
      <td>[!UICONTROL 説明]</td>
      <td>description</td>
    </tr>
  </tbody>
</table>

以下の取引先責任者フィールドは、内部で使用するために同期されます。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL 所有者]</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 作成日]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社名]</td>
      <td>parentcustomerid</td>
    </tr>
  </tbody>
</table>

## アカウントフィールド {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo フィールド</th>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL アカウント（a）]</td>
      <td>[!UICONTROL アカウント]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求先住所]</td>
      <td>[!UICONTROL 住所 1：番地 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求先住所（市区町村）]</td>
      <td>[!UICONTROL 住所 1：市区町村]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求先住所（国）]</td>
      <td>[!UICONTROL 住所 1：国／地域]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求先住所（郵便番号）]</td>
      <td>[!UICONTROL 住所 1：郵便番号]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 請求先住所 2]</td>
      <td>[!UICONTROL 住所 1：番地 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 請求先住所 3]</td>
      <td>[!UICONTROL 住所 1：番地 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL 代表電話]</td>
      <td>[!UICONTROL 代表電話]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL ビジネスタイプ]</td>
      <td>[!UICONTROL ビジネスタイプ]</td>
      <td>businesstypecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft アカウント番号]</td>
      <td>[!UICONTROL アカウント番号]</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 企業ステータス]</td>
      <td>[!UICONTROL ステータス]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 年間収益]</td>
      <td>[!UICONTROL 年間収益]</td>
      <td>revenue</td>
    </tr>
    <tr>
      <td>[!UICONTROL 企業注記]</td>
      <td>[!UICONTROL 説明]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL 業界]</td>
      <td>[!UICONTROL 業界]</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC コード]</td>
      <td>[!UICONTROL SIC コード]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Web サイト]</td>
      <td>[!UICONTROL Web サイト]</td>
      <td>website</td>
    </tr>
    <tr>
      <td>[!UICONTROL 従業員数]</td>
      <td>[!UICONTROL 従業員数]</td>
      <td>numberofemployees</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC コード]</td>
      <td>[!UICONTROL SIC コード]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社]</td>
      <td>[!UICONTROL アカウント名]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL 従業員数]</td>
      <td>[!UICONTROL 従業員数]</td>
      <td>numberofemployees</td>
    </tr>
  </tbody>
</table>

以下のアカウントフィールドは、内部で使用するために同期されます。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL 所有者]</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 作成日]</td>
      <td>createdon</td>
    </tr>
  </tbody>
</table>

## 商談フィールド {#opportunity-fields}

<table>
  <colgroup>
    <col/>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo フィールド</th>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL クローズする確率]</td>
      <td>[!UICONTROL 確率]</td>
      <td>closeprobability</td>
    </tr>
    <tr>
      <td>[!UICONTROL ステージ]</td>
      <td>[!UICONTROL ステータス]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 実際のクローズ日]</td>
      <td>[!UICONTROL 実際のクローズ日]</td>
      <td>actualclosedate</td>
    </tr>
    <tr>
      <td>[!UICONTROL 名前]</td>
      <td>[!UICONTROL トピック]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL 予測値]</td>
      <td>[!UICONTROL 予測収益]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL 説明]</td>
      <td>[!UICONTROL 説明]</td>
      <td>description</td>
    </tr>
  </tbody>
</table>

以下のアカウントフィールドは、内部で使用するために同期されます。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>MS Dynamics フィールド</th>
      <th>MS Dynamics API 名</th>
    </tr>
    <tr>
      <td>[!UICONTROL 所有者]</td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 商談]</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL 見込み顧客]</td>
      <td>customerId</td>
    </tr>
  </tbody>
</table>

## Marketo の Microsoft 関連システムフィールド（読み取り専用） {#microsoft-related-system-fields}

以下のフィールドは Marketo で作成されますが、ユーザが調整することはできません。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Marketo フィールド</th>
      <th>説明</th>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft タイプ]</td>
      <td>リードまたは取引先責任者。空の場合、リードは Marketo に人物としてのみ存在します</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft の作成日]</td>
      <td>[!DNL MS Dynamics] で作成された日付（Marketo で作成された日付とは異なる場合があります）</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft 削除済み]</td>
      <td>以前は Microsoft に存在したが、削除され、現在は Marketo にしか存在しない人物</td>
    </tr>
  </tbody>
</table>
