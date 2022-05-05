---
description: デフォルトの Veeva フィールドマッピング — Marketoドキュメント — 製品ドキュメント
title: デフォルトの Veeva フィールドマッピング
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 70%

---

# デフォルトの Veeva フィールドマッピング {#default-veeva-field-mapping}

Marketo Engageアカウントを Veeva と最初に同期すると、Marketoは組み込みの Veeva フィールドとMarketoフィールドの間でこれらの関連付けを自動的におこないます。 Marketoは、アカウントと連絡先のカスタムフィールドも同期します。

## 連絡先フィールド {#contact-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC フィールド</th>
      <th>Marketo フィールド</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>生年月日</td>
      <td>生年月日</td>
    </tr>
    <tr>
      <td>作成日</td>
      <td>SFDC 作成日</td>
    </tr>
    <tr>
      <td>連絡先の説明</td>
      <td>顧客の注記</td>
    </tr>
    <tr>
      <td>メール</td>
      <td>メールアドレス</td>
    </tr>
    <tr>
      <td>勤務先 FAX</td>
      <td>FAX 番号</td>
    </tr>
    <tr>
      <td>名</td>
      <td>名</td>
    </tr>
    <tr>
      <td>メールオプトアウト</td>
      <td>登録解除済み</td>
    </tr>
    <tr>
      <td>削除済み</td>
      <td>SFDC 削除済み</td>
    </tr>
    <tr>
      <td>姓</td>
      <td>姓</td>
    </tr>
    <tr>
      <td>リードのソース</td>
      <td>ソース</td>
    </tr>
    <tr>
      <td>リードのスコア</td>
      <td>スコア</td>
    </tr>
    <tr>
      <td>MailingCity</td>
      <td>市区町村</td>
    </tr>
    <tr>
      <td>MailingCountry</td>
      <td>国</td>
    </tr>
    <tr>
      <td>MailingPostalCode</td>
      <td>郵便番号</td>
    </tr>
    <tr>
      <td>MailingState</td>
      <td>都道府県</td>
    </tr>
    <tr>
      <td>MailingStreet</td>
      <td>住所</td>
    </tr>
    <tr>
      <td>携帯電話</td>
      <td>携帯電話番号</td>
    </tr>
    <tr>
      <td>勤務先電話</td>
      <td>電話番号</td>
    </tr>
    <tr>
      <td>敬称</td>
      <td>敬称</td>
    </tr>
    <tr>
      <td>職位</td>
      <td>職位</td>
    </tr>
  </tbody>
</table>

## アカウントフィールド {#account-fields}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>SFDC フィールド</th>
      <th>Marketo フィールド</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>年間売上高</td>
      <td>年間売上高</td>
    </tr>
    <tr>
      <td>請求先住所 (市区町村)</td>
      <td>請求先住所 (市区町村)</td>
    </tr>
    <tr>
      <td>請求先住所 (国)</td>
      <td>請求先住所 (国)</td>
    </tr>
    <tr>
      <td>請求先住所 (郵便番号)</td>
      <td>請求先住所 (郵便番号)</td>
    </tr>
    <tr>
      <td>請求先住所 (都道府県）</td>
      <td>請求先住所 (都道府県)</td>
    </tr>
    <tr>
      <td>請求先住所（番地）</td>
      <td>請求先住所</td>
    </tr>
    <tr>
      <td>アカウントの説明</td>
      <td>企業注記</td>
    </tr>
    <tr>
      <td>業界</td>
      <td>業界</td>
    </tr>
    <tr>
      <td>削除済み</td>
      <td>SFDC 削除済み</td>
    </tr>
    <tr>
      <td>アカウント名</td>
      <td>企業名</td>
    </tr>
    <tr>
      <td>従業員</td>
      <td>従業員数</td>
    </tr>
    <tr>
      <td>アカウントの電話</td>
      <td>代表電話</td>
    </tr>
    <tr>
      <td>SIC コード</td>
      <td>SIC コード</td>
    </tr>
    <tr>
      <td>アカウントサイト</td>
      <td>サイト</td>
    </tr>
    <tr>
      <td>アカウントタイプ</td>
      <td>SFDC のタイプ</td>
    </tr>
    <tr>
      <td>Web サイト</td>
      <td>Web サイト</td>
    </tr>
  </tbody>
</table>

## Marketoの Veeva 関連システムフィールド（読み取り専用） {#veeva-related-system-fields-in-marketo}

これらのフィールドはMarketoで作成されますが、お客様が調整することはできません。

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <thead>
    <tr>
      <th>フィールド</th>
      <th>説明</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Veeva Id</td>
      <td>18 文字の Salesforce ID</td>
    </tr>
    <tr>
      <td>Veeva タイプ</td>
      <td>連絡先. 空の場合、リードは Marketo にのみ存在します</td>
    </tr>
    <tr>
      <td>Veeva 作成日</td>
      <td>SFDC で作成された日付（Marketo で作成された日付とは異なる場合があります）</td>
    </tr>
    <tr>
      <td>Veeva が削除されました</td>
      <td>以前は SFDC に存在したが、削除され、現在は Marketo にしか存在しない個人</td>
    </tr>
  </tbody>
</table>
