---
unique-page-id: 5472615
description: システム管理のフィールドについて — Marketo ドキュメント — 製品ドキュメント
title: システム管理のフィールドについて
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: fc25a088005ee1d552f6e61e2fa7b953e2fde862
workflow-type: ht
source-wordcount: '523'
ht-degree: 100%

---

# システム管理のフィールドについて {#understanding-system-managed-fields}

[人物の詳細ページ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}には、Marketo によって作成される編集不可のフィールドがあることにお気付きかもしれません。そうしたフィールドのデータは、ソースも表示される値もさまざまです。

## フィールドのタイプ {#field-types}

<table><thead>
  <tr>
    <th>フィールド名</th>
    <th>定義</th>
  </tr></thead>
<tbody>
  <tr>
    <td>参照元のソースのタイプ</td>
    <td>人物または Web サイト訪問者が最初に検出された場所（例：リストのインポート、Web ページへのアクセス）</td>
  </tr>
  <tr>
    <td>参照元のソース情報</td>
    <td>その場所に関する詳細（例：リストの名前、Web ページの URL）</td>
  </tr>
  <tr>
    <td>参照元検索エンジン</td>
    <td>該当する場合には、人物を元のエントリーソースに誘導した検索エンジン</td>
  </tr>
  <tr>
    <td>参照元検索フレーズ</td>
    <td>該当する場合には、人物を元のエントリーソースに誘導した検索語句</td>
  </tr>
  <tr>
    <td>訪問者の参照元</td>
    <td>元のエントリーソースのホスト先 URL</td>
  </tr>
  <tr>
    <td>登録ソースのタイプ</td>
    <td>最初に人物として記録されるためのアクティビティが起こった場所（例：リストのインポート、Web ページへのアクセス）</td>
  </tr>
  <tr>
    <td>登録ソース情報</td>
    <td>その場所に関する詳細（例：リストの名前、Web ページの URL）</td>
  </tr>
  <tr>
    <td>匿名 IP</td>
    <td>人物の IP アドレス</td>
  </tr>
  <tr>
    <td>推測される企業</td>
    <td>人物の会社を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
  <tr>
    <td>推測される市区町村</td>
    <td>人物の市区町村を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
  <tr>
    <td>推測される都道府県／地域</td>
    <td>人物の都道府県／地域を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
  <tr>
    <td>推測される郵便番号</td>
    <td>人物の郵便番号を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
  <tr>
    <td>推測される国</td>
    <td>人物の国を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
  <tr>
    <td>推測される都市圏</td>
    <td>人物の都市圏を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
  <tr>
    <td>推測される市外局番</td>
    <td>人物の市外局番を Marketo が推測した最善の結果（IP に基づく）</td>
  </tr>
</tbody></table>

## 「参照元のソースのタイプ」と「登録ソースのタイプ」で想定される値 {#possible-values-for-original-and-registration-source-type}

想定される一部の値と、その意味は以下のとおりです。

<table><thead>
  <tr>
    <th>参照元のソースのタイプ</th>
    <th>定義</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>人物は Salesforce 同期から検出されました</td>
  </tr>
  <tr>
    <td>Web ページへのアクセス</td>
    <td>人物は Web ページから検出されました</td>
  </tr>
  <tr>
    <td>Web フォーム入力</td>
    <td>人物はフォームの入力後に検出されました</td>
  </tr>
  <tr>
    <td>リストのインポート</td>
    <td>人物はリストのインポートから検出されました</td>
  </tr>
  <tr>
    <td>新規人物</td>
    <td>人物はデータベースに手動で入力されました</td>
  </tr>
  <tr>
    <td>Web リンククリック</td>
    <td>人物はリンクをクリックした後に検出されました</td>
  </tr>
  <tr>
    <td>セールスメール</td>
    <td>リードに Sales Insight メールアドイン経由でメールが送信されました</td>
  </tr>
  <tr>
    <td>人物</td>
    <td>リードは Salesforce からリードとして同期されました</td>
  </tr>
  <tr>
    <td>取引先責任者</td>
    <td>人物は web フック から取引先責任者として同期されました</td>
  </tr>
  <tr>
    <td>Munchkin API</td>
    <td>人物は Marketo Engage Munchkin API によって検出されました</td>
  </tr>
  <tr>
    <td>ソーシャルアプリ</td>
    <td>人物はソーシャルウィジェットによって検出されました</td>
  </tr>
  <tr>
    <td>Web サービス API</td>
    <td>人物は Web サービス API によって検出されました</td>
  </tr>
  <tr>
    <td>イベントパートナー</td>
    <td>人物は同期されたウェビナーサービスによって検出されました</td>
  </tr>
  <tr>
    <td>リードの関連付け</td>
    <td>人物は人物の関連付け API 呼び出しを通じて結合されました</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>登録ソースのタイプ</th>
    <th>定義</th>
  </tr></thead>
<tbody>
  <tr>
    <td>リストのインポート</td>
    <td>リストのインポートによって人物になりました</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Salesforce の同期を通じて人物になりました</td>
  </tr>
  <tr>
    <td>Web フォーム入力</td>
    <td>フォームの記入後に人物になりました</td>
  </tr>
  <tr>
    <td>セールスメール</td>
    <td>リードに Sales Insight メールアドイン経由でメールが送信されました</td>
  </tr>
  <tr>
    <td>Web サービス API</td>
    <td>人物は SOAP／REST API を使用して作成されました</td>
  </tr>
  <tr>
    <td>新規人物</td>
    <td>人物はデータベースに手動で入力されました</td>
  </tr>
  <tr>
    <td>Munchkin API</td>
    <td>Marketo Munchkin API を通じてリードになりました</td>
  </tr>
  <tr>
    <td>ソーシャルアプリ</td>
    <td>ソーシャルウィジェットを通じて人物になりました</td>
  </tr>
  <tr>
    <td>イベントパートナー</td>
    <td>リンクされたウェビナーを通じてて人物になりました</td>
  </tr>
</tbody>
</table>
