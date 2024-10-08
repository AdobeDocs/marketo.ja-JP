---
description: OP-Scoring-Behavior - Marketo ドキュメント – 製品ドキュメント
title: OP-スコアリング-行動
feature: Programs
exl-id: c564a301-0054-431a-8f0f-0299cd91b59c
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 31%

---

# OP-スコアリング-行動 {#op-scoring-behavior}

この例は、Marketo Engageのデフォルトプログラムを使用した、行動スコアリングの高度な（トークン化された）操作プログラムです。 プログラムの「マイトークン」タブでスコアリング値を表示および編集します。 「行動スコア」というカスタムスコアフィールドが必要です。

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
   <td>01 – メンバー</td>
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
   <td>行動スコア</td>
   <td>BehaviorScore</td>
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
   <td>メール – メール内のリンクのクリック数</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>フォーム – お問い合わせフォームに入力します</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>フォーム – コンテンツフォームに入力します</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>フォーム – デフォルトのフォームに入力します</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>フォーム – イベントフォームに入力します</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web – 任意のPDFをダウンロード</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web - PPC スコアリング</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web – 主要な Web ページを訪問</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web - 1 日で複数の Web ページを訪問</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ライブイベント – 出席</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>展示会 – 影響</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>展示会 – 来場ブース</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ウェビナー – 出席</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>スコアを減らす – アクティビティなし</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>スコアを下げる – 望ましくない Web ページを訪問します</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>インタラクション数</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>プログラム状態の変更</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>スコアの減衰</td>
  </tr>
 </tbody> 
</table>

![](assets/op-scoring-behavior-1.png)

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
