---
description: Veeva CRM とMarketo Engageのデフォルトの Veeva フィールドマッピングについて説明します。 連絡先フィールドとアカウントフィールドのマッピング方法および同期されるカスタムフィールドを参照してください。
title: デフォルトの  [!DNL Veeva]  フィールドマッピング
exl-id: 3bf36d50-daea-431f-9537-b3007ad75945
feature: Veeva CRM
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 91%

---

# デフォルトの [!DNL Veeva] フィールドマッピング {#default-veeva-field-mapping}

Marketo Engage アカウントと [!DNL Veeva] の初回同期時に、Marketo ではビルトインの [!DNL Veeva] フィールドと Marketo フィールドの間でこれらの関連付けが自動的に行われます。Marketo は、アカウントと取引先責任者のカスタムフィールドも同期します。

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
      <td>名前（名）</td>
      <td>名前（名）</td>
    </tr>
    <tr>
      <td>メールオプトアウト</td>
      <td>配信停止完了</td>
    </tr>
    <tr>
      <td>削除済み</td>
      <td>SFDC 削除済み</td>
    </tr>
    <tr>
      <td>名前（姓）</td>
      <td>名前（姓）</td>
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

## Marketo の [!DNL Veeva] 関連システムフィールド（読み取り専用） {#veeva-related-system-fields-in-marketo}

これらのフィールドは Marketo で作成されますが、顧客は調整できません。

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
      <td>[!DNL Veeva] ID</td>
      <td>18 文字の [!DNL Salesforce] ID</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] タイプ</td>
      <td>取引先責任者。空の場合、リードは Marketo に人物としてのみ存在します</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] 作成日</td>
      <td>SFDC で作成された日付（Marketo で作成された日付とは異なる場合があります）</td>
    </tr>
    <tr>
      <td>[!DNL Veeva] 削除済み</td>
      <td>以前は SFDC に存在したが、削除され、現在は Marketo にしか存在しない人物</td>
    </tr>
  </tbody>
</table>
