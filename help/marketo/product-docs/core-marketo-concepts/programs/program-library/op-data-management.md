---
description: データ管理運用プログラムテンプレート。 データベースをクリーンで最新の状態に保つために使用します。
title: OP-データ管理
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
TQID: https://experienceleague.adobe.com/EGzqLIOGFIpRAB2OoDhRBTheiHBtitfI29T8TvZQNp0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 27%

---

# OP-データ管理 {#op-data-management}

これは、Marketo Engage データベース内のレコードのデータの一貫性を管理する際に役立つ、デフォルトプログラムを使用した簡単な運用データ管理ベストプラクティスワークフローの例です。

詳しい戦略支援またはプログラムのカスタマイズについては、Adobe アカウントチームにお問い合わせいただくか、[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} ページをご覧ください。

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
   <td>Normalize Country - アメリカ合衆国</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Normalize Country - イギリス</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>設定された値をTrueに設定</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Set Is Partner to True</td>
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
   <td>リストの読み込みからの新規ユーザー</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>ライブイベントからの新規ユーザー</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Online Advertisingの新しい人物</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>展示会からの新しい人物</td>
  </tr>
   <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Web コンテンツから新しい人物</td>
  </tr>
   <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Web リクエストからの新規ユーザー</td>
  </tr>
   <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>ウェビナーの新規参加者</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>人物Source Nightly バッチ（高トラフィックインスタンスの場合）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>人物Source トリガー（低トラフィックインスタンスの場合）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>人物Sourceのキャプチャ</td>
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

* 構築された各キャンペーンは、ユースケースに特化したものではなく、ベストプラクティスの構築に関する例となることを目的としています。 そのため、特定の課題やデータの課題に対処するために、スマートキャンペーンを忘れずに更新する必要があります。

* 命名規則に合わせて、このプログラムの例の命名規則を更新することを検討してください。
