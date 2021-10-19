---
description: デフォルトの Dynamics フィールドマッピング - Marketo ドキュメント - 製品ドキュメント
title: デフォルトの Dynamics フィールドマッピング
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: ht
source-wordcount: '528'
ht-degree: 100%

---

# デフォルトの Dynamics フィールドマッピング {#default-dynamics-field-mapping}

Marketo アカウントを Microsoft と最初に同期すると、Marketo は組み込みの Dynamics フィールドと Marketo フィールドの間でこれらの関連付けを自動的におこないます。Marketo は、リード、アカウント、オポチュニティ、連絡先のカスタムフィールドも同期します。

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
   <td>Microsoft 作成日</td> 
   <td>作成日</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>敬称</td> 
   <td>敬称</td> 
   <td>salutation</td> 
  </tr> 
  <tr> 
   <td>名</td> 
   <td>名 </td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>ミドルネーム</td> 
   <td>ミドルネーム</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>最後</td> 
   <td>姓</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>メール</td> 
   <td>メール</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>役職</td> 
   <td>役職</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>電話</td> 
   <td>業務用電話番号</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>携帯電話</td> 
   <td>携帯電話番号</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>ファックス</td> 
   <td>ファックス</td> 
   <td>fax</td> 
  </tr> 
  <tr> 
   <td>住所</td> 
   <td>住所 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>市区町村</td> 
   <td>市区町村</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>都道府県</td> 
   <td>都道府県</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>国</td> 
   <td>国／地域</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>郵便番号</td> 
   <td>郵便番号</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>リードソース</td> 
   <td>リードのソース</td> 
   <td>leadsourcecode</td> 
  </tr> 
  <tr> 
   <td>リードステータス</td> 
   <td>ステータス</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>ステータスの理由</td> 
   <td>ステータスの理由</td> 
   <td>statuscode</td> 
  </tr> 
  <tr> 
   <td>顧客の注記</td> 
   <td>説明</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>連絡拒否</td> 
   <td>電話を許可しない</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>登録解除済み</td> 
   <td>一括メールを送信しない</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>リード評価</td> 
   <td>評価</td> 
   <td>leadqualitycode</td> 
  </tr> 
  <tr> 
   <td>Microsoft 住所 2</td> 
   <td>住所 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft 住所 3</td> 
   <td>住所 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft メール送信除外</td> 
   <td>メールを許可しない</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft ファックス送信除外</td> 
   <td>ファックスを許可しない</td> 
   <td>donotfax</td> 
  </tr> 
  <tr> 
   <td>Microsoft マーケティング資料の受領拒否</td> 
   <td>マーケティング資料</td> 
   <td>donotsendmm</td> 
  </tr> 
  <tr> 
   <td>Microsoft 自宅電話</td> 
   <td>自宅電話</td> 
   <td>telephone2</td> 
  </tr> 
  <tr> 
   <td>Microsoft 希望連絡方法</td> 
   <td>希望連絡方法</td> 
   <td>preferredcontactmethodcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft トピック</td> 
   <td>トピック</td> 
   <td>subject</td> 
  </tr> 
 </tbody> 
</table>

## 取引先責任者フィールド {#contact-fields}

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
   <td>Microsoft 作成日</td> 
   <td>作成日</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>敬称</td> 
   <td>敬称</td> 
   <td>salutation</td> 
  </tr> 
  <tr> 
   <td>名</td> 
   <td>名 </td> 
   <td>firstname</td> 
  </tr> 
  <tr> 
   <td>ミドルネーム</td> 
   <td>ミドルネーム</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>最後</td> 
   <td>姓</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>メール</td> 
   <td>メール</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>役職</td> 
   <td>役職</td> 
   <td>jobtitle</td> 
  </tr> 
  <tr> 
   <td>電話</td> 
   <td>業務用電話番号</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>携帯電話</td> 
   <td>携帯電話番号</td> 
   <td>mobilephone</td> 
  </tr> 
  <tr> 
   <td>住所</td> 
   <td>住所 1：番地 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>市区町村</td> 
   <td>住所 1：市区町村</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>都道府県</td> 
   <td>住所 1：都道府県</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>国</td> 
   <td>住所 1：国/地域</td> 
   <td>address1_country</td> 
   <tr> 
   <td>郵便番号</td> 
   <td>住所 1：郵便番号</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>リードステータス</td> 
   <td>ステータス</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>ステータスの理由</td> 
   <td>ステータスの理由</td> 
   <td>statuscode</td> 
  </tr> 
   <tr> 
   <td>連絡拒否</td> 
   <td>電話を許可しない</td> 
   <td>donotphone</td> 
  </tr> 
  <tr> 
   <td>登録解除済み</td> 
   <td>一括メールを送信しない</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft 住所 2</td> 
   <td>住所 1：番地 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Microsoft 住所 3</td> 
   <td>住所 1：番地 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft メール送信除外</td> 
   <td>メールを許可しない</td> 
   <td>donotemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft 自宅電話</td> 
   <td>自宅電話</td> 
   <td>telephone2</td> 
  </tr> 
  <tr> 
   <td>Microsoft 希望連絡方法</td> 
   <td>希望連絡方法</td> 
   <td>preferredcontactmethodcode</td> 
  </tr> 
 </tbody> 
</table>

## アカウントフィールド {#account-fields}

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
   <td>アカウント（a）</td> 
   <td>アカウント</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>請求先住所</td> 
   <td>住所 1：番地 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>請求先住所（市区町村）</td> 
   <td>住所 1：市区町村</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>請求先住所（国）</td> 
   <td>住所 1：国/地域</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>請求先住所（郵便番号）</td> 
   <td>住所 1：郵便番号</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft 請求先住所 2</td> 
   <td>住所 1：番地 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft 請求先住所 3</td> 
   <td>住所 1：番地 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>代表電話番号</td> 
   <td>代表電話番号</td> 
   <td>telephone1</td> 
  </tr> 
  <tr> 
   <td>ビジネスタイプ</td> 
   <td>ビジネスタイプ</td> 
   <td>businesstypecode</td> 
  </tr> 
  <tr> 
   <td>Microsoft アカウント番号</td> 
   <td>アカウント番号</td> 
   <td>accountnumber</td> 
  </tr> 
  <tr> 
   <td>Microsoft 企業ステータス</td> 
   <td>ステータス</td> 
   <td>statecode</td> 
  </tr> 
  <tr> 
   <td>年間収益</td> 
   <td>年間収益</td> 
   <td>revenue</td> 
  </tr> 
  <tr> 
   <td>企業注記</td> 
   <td>説明</td> 
   <td>description</td> 
  </tr> 
  <tr> 
   <td>業界</td> 
   <td>業界</td> 
   <td>industrycode</td> 
  </tr> 
  <tr> 
   <td>SIC コード</td> 
   <td>SIC コード</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>Web サイト</td> 
   <td>Web サイト</td> 
   <td>website</td> 
  </tr> 
 </tbody> 
</table>

## Marketo の Microsoft 関連システムフィールド（読み取り専用） {#microsoft-related-system-fields-in-marketo}

これらのフィールドは Marketo で作成されますが、顧客は調整できません。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo フィールド</th> 
   <th>説明</th> 
  </tr> 
  <tr> 
   <td>Microsoft タイプ</td> 
   <td>リードまたは連絡先。空の場合、リードは Marketo にのみ存在します</td> 
  </tr> 
  <tr> 
   <td>Microsoft 作成日</td> 
   <td>MS Dynamics で作成された日付（Marketo で作成された日付とは異なる場合があります）
</td> 
  </tr> 
  <tr> 
   <td>Microsoft 削除済み</td> 
   <td>以前は Microsoft に存在したが、削除され、現在は Marketo にしか存在しない個人</td> 
  </tr> 
 </tbody> 
</table>
