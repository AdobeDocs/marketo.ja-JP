---
description: OP-Data Management - Marketoドキュメント — 製品ドキュメント
title: OP-データ管理
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 6b54fe2830200c6673559a257065248390c6d212
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 28%

---

# OP-データ管理 {#op-data-management}

これは、Marketo Engage・データベース内のレコードのデータ整合性を管理するのに役立つ、デフォルト・プログラムを使用した、シンプルな運用可能なデータ管理ベスト・プラクティス・ワークフローの例です。

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
   <td>国の標準化 — 米国</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>国の標準化 — 英国</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>True に設ブロックリストに加える定</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Is Partner を True に設定</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>リストの読み込み</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ライブイベント</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>オンライン広告</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>見本市</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web コンテンツ</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ウェブリクエスト</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ウェビナー</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>リストインポートからの新規担当者</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ライブイベントからの新規担当者</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>オンライン広告の新規担当者</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>見本市の新人</td>
  </tr>
   <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web コンテンツからの新規担当者</td>
  </tr>
   <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>Web リクエストからの新規担当者</td>
  </tr>
   <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>ウェビナーからの新規担当者</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>担当者ソースの夜間バッチ（高トラフィックインスタンスの場合）</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>トリガーされた担当者のソース（低トラフィックインスタンスの場合）</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>担当者ソースのキャプチャ</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>正規化</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>レコード管理</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>ブロックリスト</td>
  </tr>
 </tbody> 
</table>

![](assets/op-data-management-1.png)

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

## ベストプラクティス {#best-practices}

* 作成された各キャンペーンは、ベストプラクティスビルドの例を示すもので、ユースケースに固有のものではありません。 スマートキャンペーンを更新し、特定の問題点やデータ上の課題に対応してください。

* 命名規則に合わせて、このプログラム例の命名規則を更新することを検討してください。
