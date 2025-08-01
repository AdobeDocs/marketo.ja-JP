---
description: OP-Data Management - Marketo ドキュメント – 製品ドキュメント
title: OP-データ管理
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 27%

---

# OP-データ管理 {#op-data-management}

これは、Marketo Engage データベース内のレコードのデータ一貫性を管理する際に役立つ、デフォルトプログラムを使用したシンプルな運用データ管理ベストプラクティスワークフローの例です。

詳細な方法に関するサポートや、プログラムのカスタマイズに関するヘルプについては、Adobe アカウントチームに問い合わせるか、[Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} のページを参照してください。

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
   <td>国を正規化 – 米国</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>国を正規化 – 英国</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>True にブロックリストに加える</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>パートナーを True に設定</td>
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
   <td>リストの読み込みから新規人物</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>ライブイベントからの新しいユーザー</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>オンラインAdvertisingからの新しいユーザー</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>見本市の新人</td>
  </tr>
   <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Web コンテンツからの新しいユーザー</td>
  </tr>
   <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>Web リクエストからの新しいユーザー</td>
  </tr>
   <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>ウェビナーの新しいユーザー</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>人物Source夜間バッチ（高トラフィックインスタンスの場合）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>人物Sourceがトリガーされます（低トラフィックインスタンスの場合）</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>人物のSourceをキャプチャ</td>
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
