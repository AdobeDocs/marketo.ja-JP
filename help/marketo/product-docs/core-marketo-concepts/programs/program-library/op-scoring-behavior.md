---
description: OP スコア付け動作 — Marketoドキュメント — 製品ドキュメント
title: OP-スコアリング-行動
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 0f71600b18315feb3ef32e95dfb108b09c4cb79f
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 30%

---

# OP-スコアリング-行動 {#op-scoring-behavior}

この例は、「デフォルトプログラム」を使用した行動スコアリングの高度な（トークン化された）運用プログラムのMarketo Engageです。 プログラムの「マイトークン」タブで、スコアリング値を表示および編集します。 「行動スコア」と呼ばれるカスタムスコアフィールドが必要です。

戦略に関するサポートやプログラムのカスタマイズについては、Adobeアカウントチームにお問い合わせいただくか、 [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} ページに貼り付けます。

## チャネルサマリ {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>チャネル</th> 
   <th>メンバーシップステータス</th>
   <th>アナリティクス動作</th>
   <th>プログラムのタイプ</th>
  </tr> 
  <tr> 
   <td>オペレーショナル</td> 
   <td>01 — メンバー</td>
   <td>オペレーショナル</td>
   <td>デフォルト</td>
  </tr>
 </tbody> 
</table>

## 前提条件のフィールド {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>タイプ</th> 
   <th>フレンドリ名</th>
   <th>API 名</th>
  </tr>
  <tr> 
   <td>Score</td> 
   <td>行動スコア</td>
   <td>BehaviorScore</td>
  </tr>
 </tbody> 
</table>

## プログラムに次のアセットが含まれています {#program-contains-the-following-assets}

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
   <td>電子メール — 電子メール内のリンクをクリック</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>フォーム — 連絡先フォームの入力</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Form - Fills Out Content Form</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Form - Fills Out Default Form</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>フォーム — イベントフォームの入力</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web — 任意のPDFをダウンロード</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web - PPC スコアリング</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web — 主要な Web ページを訪問</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web - 1 日に複数の Web ページを訪問</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ライブイベント — 出席済み</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>トレードショー — 影響</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>展示会 — 訪問ブース</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>オンラインセミナ — 出席</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>スコアを減らす — アクティビティなし</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>スコアの減少 — 望ましくない Web ページの訪問回数</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>インタラクション数</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>プログラムステータスの変更</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>スコア減衰</td>
  </tr>
 </tbody> 
</table>

プログラムのスクリーンショット

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
   <td><code>{{my.Decrease Score - No Activity}}</code></td>
   <td>-10</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Decrease Score - Visits Undesirable Web Pages}}</code></td>
   <td>-5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Email - Clicks Link}}</code></td>
   <td>+2</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Form - Fills Out Contact Form}}</code></td>
   <td>+30</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Form - Fills Out Content Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Form - Fills Out Default Form}}</code></td>
   <td>+10</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Form - Fills-out Event Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Live Event - Attended}}</code></td>
   <td>+30</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Tradeshow - Influenced}}</code></td>
   <td>+20</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Tradeshow - Visited Booth}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Web - Downloaded Any PDF}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Web - PPC Scoring}}</code></td>
   <td>+15</td>
  </tr>
   <tr> 
   <td>Score</td> 
   <td><code>{{my.Web - Visits Key Web Pages}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Web - Visits Multiple Web Pages in 1 Day}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Score</td> 
   <td><code>{{my.Webinar - Attended}}</code></td>
   <td>+20</td>
  </tr>
 </tbody> 
</table>

## 競合ルール {#conflict-rules}

* **プログラムタグ**
   * この配信登録にタグを作成 — _推奨_
   * 無視する

* **同じ名前のランディングページテンプレート**
   * 元のテンプレートをコピー — _推奨_
   * インポート先のテンプレートの使用

* **同じ名前の画像**
   * 両方のファイルを保持 — _推奨_
   * この配信登録内アイテムの置換

* **同じ名前のメールテンプレート**
   * 両方のテンプレートを保持 — _推奨_
   * 既存テンプレートの置換

競合ルールのスクリーンショット

## ベストプラクティス {#best-practices}

* 作成された各キャンペーンは、ベストプラクティスビルドの例を示すもので、ユースケースに固有のものではありません。 スマートキャンペーンを更新し、特定の問題点やデータ上の課題に対応してください。

* 命名規則に合わせて、このプログラム例の命名規則を更新することを検討してください。
