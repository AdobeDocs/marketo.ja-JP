---
description: 既定のDynamicsフィールドマッピング —Marketoドキュメント — 製品ドキュメント
title: 既定のダイナミクスフィールドマッピング
exl-id: 5f39bd0c-202e-4aa1-a0ac-49ac2554aa1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 47%

---

# 既定のダイナミックフィールドマッピング{#default-dynamics-field-mapping}

MarketoアカウントをMicrosoftと最初に同期すると、Marketoは組み込みのDynamicsとMarketoのフィールドの間でこれらの関連付けを自動的に行います。  また、Marketoは、リード、アカウント、オポチュニティ、連絡先のカスタムフィールドも同期します。

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
   <th>MS Dynamicsフィールド</th> 
   <th>MS Dynamics API名</th> 
  </tr> 
  <tr> 
   <td>Microsoft が日付作成済み</td> 
   <td>作成先</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>敬称</td> 
   <td>敬称</td> 
   <td>挨拶</td> 
  </tr> 
  <tr> 
   <td>名</td> 
   <td>名 </td> 
   <td>名</td> 
  </tr> 
  <tr> 
   <td>ミドルネーム</td> 
   <td>ミドルネーム</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>姓</td> 
   <td>姓</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>メール</td> 
   <td>メール</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>職位</td> 
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
   <td>ファックス</td> 
  </tr> 
  <tr> 
   <td>住所</td> 
   <td>番地1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>都市</td> 
   <td>都市</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>都道府県</td> 
   <td>都道府県</td> 
   <td>address1_stateorprovince</td> 
  </tr> 
  <tr> 
   <td>国</td> 
   <td>国/地域</td> 
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
   <td>担当者の注記</td> 
   <td>詳細</td> 
   <td>詳細</td> 
  </tr> 
  <tr> 
   <td>連絡拒否</td> 
   <td>電話を許可しない</td> 
   <td>ドナ</td> 
  </tr> 
  <tr> 
   <td>配信停止完了</td> 
   <td>電子メールを一括処理しない</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>リード評価</td> 
   <td>評価</td> 
   <td>leadqualitycode</td> 
  </tr> 
  <tr> 
   <td>Microsoft 住所 2</td> 
   <td>2番街</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft 住所 3</td> 
   <td>通り3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft メール送信除外</td> 
   <td>電子メールを許可しない</td> 
   <td>ドノメール</td> 
  </tr> 
  <tr> 
   <td>Microsoft ファックス送信除外</td> 
   <td>FAXを許可しない</td> 
   <td>ドノファクス</td> 
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
   <td>Microsoftが推奨する連絡方法</td> 
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
   <th>MS Dynamicsフィールド</th> 
   <th>MS Dynamics API名</th> 
  </tr> 
  <tr> 
   <td>Microsoft が日付作成済み</td> 
   <td>作成先</td> 
   <td>createdon</td> 
  </tr> 
  <tr> 
   <td>敬称</td> 
   <td>敬称</td> 
   <td>挨拶</td> 
  </tr> 
  <tr> 
   <td>名</td> 
   <td>名 </td> 
   <td>名</td> 
  </tr> 
  <tr> 
   <td>ミドルネーム</td> 
   <td>ミドルネーム</td> 
   <td>middlename</td> 
  </tr> 
  <tr> 
   <td>姓</td> 
   <td>姓</td> 
   <td>lastname</td> 
  </tr> 
  <tr> 
   <td>メール</td> 
   <td>メール</td> 
   <td>emailaddress1</td> 
  </tr> 
  <tr> 
   <td>職位</td> 
   <td>職位</td> 
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
   <td>住所 1：通り 1</td> 
   <td>address1_line1</td> 
   <tr> 
   <td>都市</td> 
   <td>住所 1：都市</td> 
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
   <td>住所1:郵便番号</td> 
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
   <td>ドナ</td> 
  </tr> 
  <tr> 
   <td>配信停止完了</td> 
   <td>電子メールを一括処理しない</td> 
   <td>donotbulkemail</td> 
  </tr> 
  <tr> 
   <td>Microsoft 住所 2</td> 
   <td>住所 1：通り 2</td> 
   <td>address1_line2</td> 
  </tr> 
   <tr> 
   <td>Microsoft 住所 3</td> 
   <td>住所 1：通り 3</td> 
   <td>address1_line3</td> 
  </tr> 
  <tr> 
   <td>Microsoft メール送信除外</td> 
   <td>電子メールを許可しない</td> 
   <td>ドノメール</td> 
  </tr> 
  <tr> 
   <td>Microsoft 自宅電話</td> 
   <td>自宅電話</td> 
   <td>telephone2</td> 
  </tr> 
  <tr> 
   <td>Microsoftが推奨する連絡方法</td> 
   <td>好ましい接触方法</td> 
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
   <th>MS Dynamicsフィールド</th> 
   <th>MS Dynamics API名</th> 
  </tr> 
  <tr> 
   <td>アカウント（a）</td> 
   <td>アカウント</td> 
   <td>accountid</td> 
  </tr> 
  <tr> 
   <td>請求先住所</td> 
   <td>住所 1：通り 1</td> 
   <td>address1_line1</td> 
  </tr> 
  <tr> 
   <td>請求先住所 (都市)</td> 
   <td>住所 1：都市</td> 
   <td>address1_city</td> 
  </tr> 
  <tr> 
   <td>請求先住所 (国)</td> 
   <td>住所 1：国/地域</td> 
   <td>address1_country</td> 
  </tr> 
  <tr> 
   <td>請求先住所 (郵便番号)</td> 
   <td>住所1:郵便番号</td> 
   <td>address1_postalcode</td> 
  </tr> 
  <tr> 
   <td>Microsoft 請求先住所 2</td> 
   <td>住所 1：通り 2</td> 
   <td>address1_line2</td> 
  </tr> 
  <tr> 
   <td>Microsoft 請求先住所 3</td> 
   <td>住所 1：通り 3</td> 
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
   <td>Microsoftアカウント番号</td> 
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
   <td>収益</td> 
  </tr> 
  <tr> 
   <td>企業注記</td> 
   <td>詳細</td> 
   <td>詳細</td> 
  </tr> 
  <tr> 
   <td>業界</td> 
   <td>業界</td> 
   <td>産業コード</td> 
  </tr> 
  <tr> 
   <td>SIC コード</td> 
   <td>SIC コード</td> 
   <td>sic</td> 
  </tr> 
  <tr> 
   <td>ウェブサイト</td> 
   <td>ウェブサイト</td> 
   <td>webサイト</td> 
  </tr> 
 </tbody> 
</table>

## MarketoのMicrosoft関連システムフィールド（読み取り専用） {#microsoft-related-system-fields-in-marketo}

これらのフィールドはMarketoで作成されますが、顧客は調整できません。

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Marketo フィールド</th> 
   <th>詳細</th> 
  </tr> 
  <tr> 
   <td>Microsoft タイプ</td> 
   <td>リードまたは連絡先。 リードが空の場合、リードはMarketoの個人としてのみ存在します</td> 
  </tr> 
  <tr> 
   <td>Microsoft が日付作成済み</td> 
   <td>MS Dynamicsで作成された日付(Marketoで作成された日付と異なる可能性があります)</td> 
  </tr> 
  <tr> 
   <td>Microsoftが削除されました</td> 
   <td>以前はマイクロソフトにいたが、削除され、現在はMarketoにしか住んでいない人</td> 
  </tr> 
 </tbody> 
</table>
