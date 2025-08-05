---
description: OP-Acquisition-API - Marketo ドキュメント – 製品ドキュメント
title: OP-Acquisition-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 21%

---

# OP-Acquisition-API {#op-acquisition-api}

このサンプルプログラムは、Marketo Engageのデフォルトプログラムを使用して API ソースからレコードの取得をトラッキングする運用プロセス用です。

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
   <td>取得の設定 – バッチ</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>取得の設定 – トリガー</td>
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

* データ管理に追いつく必要がある場合は、最初にバッチキャンペーンを実行します。

* 同様のプログラムを利用して、すべての入力ソースにわたってベストプラクティスとの整合性を確保し、CRM またはデータ統合を含めることを検討してください。

* チャネル固有のチャネルマーケティングの取り組み内で、必要に応じて獲得をキャプチャしてください。
