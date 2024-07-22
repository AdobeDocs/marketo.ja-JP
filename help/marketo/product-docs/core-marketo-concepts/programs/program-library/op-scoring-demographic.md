---
description: OP-Scoring-Demographic - Marketo ドキュメント – 製品ドキュメント
title: OP-スコアリング-デモグラフィック
feature: Programs
exl-id: ed11616e-b587-4d03-b293-9cc9fa3c1699
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 36%

---

# OP-スコアリング-デモグラフィック {#op-scoring-demographic}

これは、人口統計スコアリング用のMarketo Engageのデフォルトプログラムを利用した、高度な（トークン化された）運用プログラムの例です。 プログラムの「マイトークン」タブでスコアリング値を表示および編集します。 「デモグラフィックスコア」というカスタムスコアフィールドが必要です。

詳細な手順に関するサポートやプログラムのカスタマイズについては、Adobeアカウントチームに問い合わせるか、[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} のページを参照してください。

## チャネルサマリ {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>チャネル</th> 
   <th>メンバーシップのステータス</th>
   <th>アナリティクス動作</th>
   <th>プログラムのタイプ</th>
  </tr> 
  <tr> 
   <td>オペレーショナル</td> 
   <td>01 - メンバー</td>
   <td>オペレーショナル</td>
   <td>デフォルト</td>
  </tr>
 </tbody> 
</table>

## 必須フィールド {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>タイプ</th> 
   <th>フレンドリ名</th>
   <th>API 名</th>
  </tr>
  <tr> 
   <td>Score</td> 
   <td>デモグラフィックスコア</td>
   <td>DemographicScore</td>
  </tr>
 </tbody> 
</table>

## プログラムには、次のAssetsが含まれています {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>タイプ</th> 
   <th>テンプレート名</th>
   <th>アセット名</th>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>汎用電子メールドメイン</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>名が無効です</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>無効な名が更新されました</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>姓が無効です</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>更新された姓が無効です</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>年間収益</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>業界</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>役職</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>従業員数</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ソース</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>汎用電子メールドメイン</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>名が無効です</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>姓が無効です</td>
  </tr>
 </tbody> 
</table>

![](assets/op-scoring-demographic-1.png)

## 含まれるマイトークン {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>トークンのタイプ</th> 
   <th>トークン名</th>
   <th>値</th>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Annual Revenue - High}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Annual Revenue - Low}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Annual Revenue - Mid}}</code></td>
   <td>+10</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Generic Email Domain}}</code></td>
   <td>-2</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Industry - High}}</code></td>
   <td>+10</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Industry - Low}}</code></td>
   <td>+6</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Industry - Mid}}</code></td>
   <td>+8</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Invalid First Name}}</code></td>
   <td>-5</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Invalid First Name Updated}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Invalid Last Name}}</code></td>
   <td>-5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Invalid Last Name Updated}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Job Title - High}}</code></td>
   <td>+15</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Job Title - Low}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Job Title - Mid}}</code></td>
   <td>+10</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Lead Source - High}}</code></td>
   <td>+20</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Lead Source - Low}}</code></td>
   <td>+8</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Lead Source - Mid}}</code></td>
   <td>+10</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Number of Employees}}</code></td>
   <td>+5</td>
  </tr>
 </tbody> 
</table>

## 競合ルール {#conflict-rules}

* **プログラムタグ**
   * このサブスクリプションにタグを作成 – _推奨_
   * 無視

* **同じ名前のランディングページテンプレート**
   * 元のテンプレートをコピー – _推奨_
   * インポート先のテンプレートの使用

* **同じ名前の画像**
   * 両方のファイルを保持 – _推奨_
   * このサブスクリプション内アイテムの置換

* **同じ名前のメールテンプレート**
   * 両方のテンプレートを保持 – _推奨_
   * 既存テンプレートの置換

## ベストプラクティス {#best-practices}

* 構築された各キャンペーンは、ユースケースに固有ではなく、ベストプラクティスのビルドの例となることを目的としています。 特定のペイン ポイントとデータの課題に対処できるように、スマートキャンペーンを必ず更新してください。

* 命名規則に合わせて、このプログラムの例の命名規則を更新することを検討してください。
