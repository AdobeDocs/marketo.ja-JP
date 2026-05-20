---
description: 獲得API運用プログラムテンプレート： API経由でリードを獲得するために使用します。
title: OP-Acquisition-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
TQID: https://experienceleague.adobe.com/a-4w7mJg44cvotVtX2qwx1e4p8SKIbQU1jPWyQ0BzUA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: df401a2a-327d-468c-a5e4-b7b7ccd071a0
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 21%

---

# OP-Acquisition-API {#op-acquisition-api}

このサンプルプログラムは、Marketo Engage デフォルトプログラムを使用してAPI ソースからレコードを取得する操作プロセスを対象としています。

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
   <td>Set Acquisition - Batch</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Set Acquisition - トリガー</td>
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
   * このサブスクリプションでタグを作成 – _おすすめ_
   * 無視

* **同じ名前のランディングページテンプレート**
   * 元のテンプレートをコピー – _おすすめ_
   * インポート先のテンプレートの使用

* **同じ名前の画像**
   * 両方のファイルを保持 – _推奨_
   * このサブスクリプション内アイテムの置換

* **同じ名前のメールテンプレート**
   * 両方のテンプレートを保持 – _推奨_
   * 既存テンプレートの置換

## ベストプラクティス {#best-practices}

* データ管理で追いつく必要がある場合は、まずバッチキャンペーンを実行します。

* CRMやデータ統合を含めるために、あらゆる入力ソースをまたいでベストプラクティスを統一するために、同様のプログラムを利用することを検討します。

* チャネルごとのチャネルマーケティング施策では、必要に応じて獲得を確保します。
