---
description: OP-Deliverability Management - Marketoドキュメント — 製品ドキュメント
title: OP-配信品質管理
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 21%

---

# OP-配信品質管理 {#op-deliverability-management}

これは、Marketo Engageのデフォルトプログラムを利用した配信品質管理のベストプラクティスワークフローの例で、E メール配信品質の現在の状態を確認し、慢性的なバウンスと非レスポンダーを管理します。

>[!NOTE]
>
>読み込むには、カスタム文字列フィールド「マーケティングの中断理由」が必要です。 [詳細情報](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

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
   <td>文字列</td> 
   <td>マーケティング中断の理由</td>
   <td>MarketingSuspendedReason</td>
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
   <td>慢性的な非対応者のマーケティング停止</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>時系列的にバウンスするメールのマーケティング停止</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>メールの更新後に「メールが無効です」をリセット</td>
  </tr>
  <tr> 
   <td>スマートキャンペーン</td> 
   <td> </td>
   <td>メールの更新後に「マーケティングを中断」をリセット</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>管理</td>
  </tr>
  <tr> 
   <td>フォルダー</td> 
   <td> </td>
   <td>レビュー</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

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
