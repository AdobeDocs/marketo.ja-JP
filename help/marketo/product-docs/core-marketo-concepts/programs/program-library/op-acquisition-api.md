---
description: OP-Acquisition-API - Marketoドキュメント — 製品ドキュメント
title: OP-Acquisition-API
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 21%

---

# OP-Acquisition-API {#op-acquisition-api}

このサンプルプログラムは、オペレーショナルプロセスが、Marketo Engageのデフォルトプログラムを使用して API ソースからのレコードの取得を追跡するためのものです。

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
   <td>獲得の設定 — バッチ</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>獲得の設定 —トリガー</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>キャンペーン（すべてのスマートキャンペーンを含む）</td>
  </tr>
 </tbody> 
</table>

![](assets/op-acquisition-api-1.png)

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

* データ管理に追いつく必要がある場合は、まずバッチキャンペーンを実行します。

* 類似したプログラムを使用して、すべての入力ソースにわたるベストプラクティスと連携し、CRM またはデータ統合を含めることを検討します。

* チャネル固有のチャネルマーケティングイニシアチブ内で、必要に応じて獲得をキャプチャするようにしてください。
