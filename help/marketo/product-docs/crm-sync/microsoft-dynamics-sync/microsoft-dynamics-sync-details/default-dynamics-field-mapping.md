---
description: デフォルトの Dynamics フィールドマッピング - Marketo ドキュメント - 製品ドキュメント
title: デフォルトの Dynamics フィールドマッピング
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1036'
ht-degree: 28%

---

# デフォルトの Dynamics フィールドマッピング {#default-dynamics-field-mapping}

Marketo Engage アカウントを最初にMicrosoftと同期すると、Marketoによって、組み込みの Dynamics フィールドとMarketo フィールドの間で自動的にこれらの関連付けが行われます。  Marketo は、リード、アカウント、商談、取引先責任者のカスタムフィールドも同期します。

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
      <td>[!UICONTROL Microsoft作成日 ]</td>
      <td>[!UICONTROL の作成日 ]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL 敬称 ]</td>
      <td>[!UICONTROL 敬称 ]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL 先頭 ]</td>
      <td>[!UICONTROL の名 ]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL 中央 ]</td>
      <td>[!UICONTROL のミドルネーム ]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL の最後 ]</td>
      <td>[!UICONTROL の姓 ]</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>[!UICONTROL メール ]</td>
      <td>[!UICONTROL メール ]</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 役職 ]</td>
      <td>[!UICONTROL 役職 ]</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>[!UICONTROL 電話 ]</td>
      <td>[!UICONTROL ビジネス電話 ]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL モバイル ]</td>
      <td>[!UICONTROL 携帯電話 ]</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>[!UICONTROL FAX]</td>
      <td>[!UICONTROL FAX]</td>
      <td>fax</td>
    </tr>
    <tr>
      <td>[!UICONTROL アドレス ]</td>
      <td>[!UICONTROL 通り 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[！市区町村 ]</td>
      <td>[！市区町村 ]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL の状態 ]</td>
      <td>[!UICONTROL 都道府県 ]</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>[!UICONTROL 国 ]</td>
      <td>[!UICONTROL の国/地域 ]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL 郵便番号 ]</td>
      <td>[!UICONTROL 郵便番号 ]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL ユーザーSource]</td>
      <td>[!UICONTROL リードSource]</td>
      <td>leadsourcecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物ステータス ]</td>
      <td>[!UICONTROL の状態 ]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 状態の理由 ]</td>
      <td>[!UICONTROL 状態の理由 ]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物メモ ]</td>
      <td>[!UICONTROL の説明 ]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL を呼び出さない ]</td>
      <td>[!UICONTROL で電話を許可しない ]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL の購読解除 ]</td>
      <td>[!UICONTROL で電子メールを一括で送信しない ]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物評価 ]</td>
      <td>[!UICONTROL 評価 ]</td>
      <td>leadqualitycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft アドレス 2]</td>
      <td>[!UICONTROL 通り 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft アドレス 3]</td>
      <td>[!UICONTROL 通り 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoftがメールを送信しない ]</td>
      <td>[!UICONTROL でメールを許可しない ]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL で FAX を許可しない ]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoftがマーケティング資料を送信しない ]</td>
      <td>[!UICONTROL マーケティング資料 ]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft ホーム電話 ]</td>
      <td>[!UICONTROL ホーム電話 ]</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft推奨の連絡方法 ]</td>
      <td>[!UICONTROL 推奨の連絡方法 ]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft トピック ]</td>
      <td>[!UICONTROL トピック ]</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最終注目の瞬間の日付 ]</td>
      <td>[!UICONTROL 最終注目の瞬間の日付 ]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最後の興味深いモーメントの説明 ]</td>
      <td>[!UICONTROL 最後の興味深いモーメントの説明 ]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最後の興味深いモーメント ソース ]</td>
      <td>[!UICONTROL 最後の興味深いモーメント ソース ]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最後の興味深いモーメント タイプ ]</td>
      <td>[!UICONTROL 最後の興味深いモーメント タイプ ]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社 ]</td>
      <td>[!UICONTROL 会社名 ]</td>
      <td>companyname</td>
    </tr>
    <tr>
      <td>[!UICONTROL 相対スコア ]</td>
      <td>[!UICONTROL 相対スコア ]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL の優先度 ]</td>
      <td>[!UICONTROL の優先度 ]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL の相対的な緊急度 ]</td>
      <td>[!UICONTROL 緊急度 ]</td>
      <td>mkt_ecqurency</td>
    </tr>
    <tr>
      <td>[!UICONTROL 件名 ]</td>
      <td>[!UICONTROL トピック ]</td>
      <td>subject</td>
    </tr>
    <tr>
      <td>[!UICONTROL の年間売上高 ]</td>
      <td>[!UICONTROL の年間売上高 ]</td>
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
      <td>[!UICONTROL 所有者 ] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL の作成日 ]</td>
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
      <td>[!UICONTROL Microsoft作成日 ]</td>
      <td>[!UICONTROL の作成日 ]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL 敬称 ]</td>
      <td>[!UICONTROL 敬称 ]</td>
      <td>salutation</td>
    </tr>
    <tr>
      <td>[!UICONTROL 先頭 ]</td>
      <td>[!UICONTROL の名 ]</td>
      <td>firstname</td>
    </tr>
    <tr>
      <td>[!UICONTROL 中央 ]</td>
      <td>[!UICONTROL のミドルネーム ]</td>
      <td>middlename</td>
    </tr>
    <tr>
      <td>[!UICONTROL の最後 ]</td>
      <td>[!UICONTROL の姓 ]</td>
      <td>lastname</td>
    </tr>
    <tr>
      <td>[!UICONTROL メール ]</td>
      <td>[!UICONTROL メール ]</td>
      <td>emailaddress1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 役職 ]</td>
      <td>[!UICONTROL 役職 ]</td>
      <td>jobtitle</td>
    </tr>
    <tr>
      <td>[!UICONTROL 電話 ]</td>
      <td>[!UICONTROL ビジネス電話 ]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL モバイル ]</td>
      <td>[!UICONTROL 携帯電話 ]</td>
      <td>mobilephone</td>
    </tr>
    <tr>
      <td>[!UICONTROL アドレス ]</td>
      <td>[!UICONTROL 住所 1：番地 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[！市区町村 ]</td>
      <td>[!UICONTROL 住所 1：市区町村 ]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL の状態 ]</td>
      <td>[!UICONTROL 住所 1：都道府県 ]</td>
      <td>address1_stateorprovince</td>
    </tr>
    <tr>
      <td>[!UICONTROL 国 ]</td>
      <td>[!UICONTROL 住所 1：国/地域 ]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL 郵便番号 ]</td>
      <td>[!UICONTROL 住所 1：郵便番号 ]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物ステータス ]</td>
      <td>[!UICONTROL の状態 ]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 状態の理由 ]</td>
      <td>[!UICONTROL 状態の理由 ]</td>
      <td>statuscode</td>
    </tr>
    <tr>
      <td>[!UICONTROL を呼び出さない ]</td>
      <td>[!UICONTROL で電話を許可しない ]</td>
      <td>donotphone</td>
    </tr>
    <tr>
      <td>[!UICONTROL の購読解除 ]</td>
      <td>[!UICONTROL で電子メールを一括で送信しない ]</td>
      <td>donotbulkemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft アドレス 2]</td>
      <td>[!UICONTROL 住所 1：番地 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft アドレス 3]</td>
      <td>[!UICONTROL 住所 1：番地 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoftがメールを送信しない ]</td>
      <td>[!UICONTROL でメールを許可しない ]</td>
      <td>donotemail</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft ホーム電話 ]</td>
      <td>[!UICONTROL ホーム電話 ]</td>
      <td>telephone2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft推奨の連絡方法 ]</td>
      <td>[!UICONTROL 推奨の連絡方法 ]</td>
      <td>preferredcontactmethodcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最終注目の瞬間の日付 ]</td>
      <td>[!UICONTROL 最終注目の瞬間の日付 ]</td>
      <td>mkt_lastinterestingmomentdate</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最後の興味深いモーメント タイプ ]</td>
      <td>[!UICONTROL 最後の興味深いモーメント タイプ ]</td>
      <td>mkt_lastinterestingmomenttype</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最後の興味深いモーメント ソース ]</td>
      <td>[!UICONTROL 最後の興味深いモーメント ソース ]</td>
      <td>mkt_leadinterestingmomentsource</td>
    </tr>
    <tr>
      <td>[!UICONTROL 最後の興味深いモーメントの説明 ]</td>
      <td>[!UICONTROL 最後の興味深いモーメントの説明 ]</td>
      <td>mkt_lastinterestingmomentdesc</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoftがマーケティング資料を送信しない ]</td>
      <td>[!UICONTROL マーケティング資料 ]</td>
      <td>donotsendmm</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>[!UICONTROL Microsoft Do Not Fax]</td>
      <td>donotfax</td>
    </tr>
    <tr>
      <td>[!UICONTROL の優先度 ]</td>
      <td>[!UICONTROL の優先度 ]</td>
      <td>mkt_priority</td>
    </tr>
    <tr>
      <td>[!UICONTROL の相対的な緊急度 ]</td>
      <td>[!UICONTROL 緊急度 ]</td>
      <td>mkt_ecqurency</td>
    </tr>
    <tr>
      <td>[!UICONTROL 相対スコア ]</td>
      <td>[!UICONTROL 相対スコア ]</td>
      <td>mkt_relativescore</td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物メモ ]</td>
      <td>[!UICONTROL の説明 ]</td>
      <td>説明 </td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物スコア ]</td>
      <td>[!UICONTROL リードスコア ]</td>
      <td>mkt_leadscore</td>
    </tr>
    <tr>
      <td>[!UICONTROL 人物メモ ]</td>
      <td>[!UICONTROL の説明 ]</td>
      <td>説明 </td>
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
      <td>[!UICONTROL 所有者 ] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL の作成日 ]</td>
      <td>createdon</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社名 ]</td>
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
      <td>[!UICONTROL アカウント （a） ]</td>
      <td>[!UICONTROL アカウント ]</td>
      <td>accountid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求先住所 ]</td>
      <td>[!UICONTROL 住所 1：番地 1]</td>
      <td>address1_line1</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求都市 ]</td>
      <td>[!UICONTROL 住所 1：市区町村 ]</td>
      <td>address1_city</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求国 ]</td>
      <td>[!UICONTROL 住所 1：国/地域 ]</td>
      <td>address1_country</td>
    </tr>
    <tr>
      <td>[!UICONTROL 請求郵便番号 ]</td>
      <td>[!UICONTROL 住所 1：郵便番号 ]</td>
      <td>address1_postalcode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft請求先住所 2]</td>
      <td>[!UICONTROL 住所 1：番地 2]</td>
      <td>address1_line2</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft請求先住所 3]</td>
      <td>[!UICONTROL 住所 1：番地 3]</td>
      <td>address1_line3</td>
    </tr>
    <tr>
      <td>[!UICONTROL メイン電話 ]</td>
      <td>[!UICONTROL メイン電話 ]</td>
      <td>telephone1</td>
    </tr>
    <tr>
      <td>[!UICONTROL ビジネス タイプ ]</td>
      <td>[!UICONTROL ビジネス タイプ ]</td>
      <td>businesstypecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft アカウント番号 ]</td>
      <td>[!UICONTROL アカウント番号 ]</td>
      <td>accountnumber</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft会社ステータス ]</td>
      <td>[!UICONTROL の状態 ]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL の年間売上高 ]</td>
      <td>[!UICONTROL の年間売上高 ]</td>
      <td>revenue</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社注記 ]</td>
      <td>[!UICONTROL の説明 ]</td>
      <td>description</td>
    </tr>
    <tr>
      <td>[!UICONTROL 業界 ]</td>
      <td>[!UICONTROL 業界 ]</td>
      <td>industrycode</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC コード ]</td>
      <td>[!UICONTROL SIC コード ]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL Web サイト ]</td>
      <td>[!UICONTROL Web サイト ]</td>
      <td>website</td>
    </tr>
    <tr>
      <td>[!UICONTROL 従業員数 ]</td>
      <td>[!UICONTROL 従業員数 ]</td>
      <td>numberofemployees</td>
    </tr>
    <tr>
      <td>[!UICONTROL SIC コード ]</td>
      <td>[!UICONTROL SIC コード ]</td>
      <td>sic</td>
    </tr>
    <tr>
      <td>[!UICONTROL 会社 ]</td>
      <td>[!UICONTROL アカウント名 ]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL 従業員数 ]</td>
      <td>[!UICONTROL 従業員数 ]</td>
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
      <td>[!UICONTROL 所有者 ] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL の作成日 ]</td>
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
      <td>[!UICONTROL 閉じる確率 ]</td>
      <td>[!UICONTROL の確率 ]</td>
      <td>closeprobability</td>
    </tr>
    <tr>
      <td>[!UICONTROL ステージ ]</td>
      <td>[!UICONTROL の状態 ]</td>
      <td>statecode</td>
    </tr>
    <tr>
      <td>[!UICONTROL 実際のクローズ日 ]</td>
      <td>[!UICONTROL 実際のクローズ日 ]</td>
      <td>actualclosedate</td>
    </tr>
    <tr>
      <td>[!UICONTROL 名 ]</td>
      <td>[!UICONTROL トピック ]</td>
      <td>name</td>
    </tr>
    <tr>
      <td>[!UICONTROL 予測値 ]</td>
      <td>[!UICONTROL のテスト。 売上高 ]</td>
      <td>estimatedValue</td>
    </tr>
    <tr>
      <td>[!UICONTROL の説明 ]</td>
      <td>[!UICONTROL の説明 ]</td>
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
      <td>[!UICONTROL 所有者 ] </td>
      <td>ownerid</td>
    </tr>
    <tr>
      <td>[!UICONTROL 商談 ]</td>
      <td>opportunityId</td>
    </tr>
    <tr>
      <td>[!UICONTROL 見込み顧客 ]</td>
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
      <td>[!UICONTROL Microsoft型 ]</td>
      <td>リードまたは取引先責任者。空の場合、リードは Marketo にのみ存在します</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoft作成日 ]</td>
      <td>[!DNL MS Dynamics] に作成された日付（Marketoで作成された日付と異なる場合があります）</td>
    </tr>
    <tr>
      <td>[!UICONTROL Microsoftが削除されました ]</td>
      <td>以前は Microsoft に存在したが、削除され、現在は Marketo にしか存在しない個人</td>
    </tr>
  </tbody>
</table>
