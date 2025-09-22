---
description: OP-Deliverability Management - Marketo ドキュメント – 製品ドキュメント
title: OP-配信品質管理
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 21%

---

# OP-配信品質管理 {#op-deliverability-management}

これは、Marketo Engageのデフォルトプログラムを使用した配信品質の管理ベストプラクティスワークフローの例で、メールの配信品質の現在の状態を確認し、慢性的なバウンスや無応答のユーザーを管理します。

>[!NOTE]
>
>インポートするには、カスタム文字列フィールド「マーケティング中断の理由」が必要です。 [詳細情報](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}。

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

## 必須フィールド {#prerequisite-fields}

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
   <td>マーケティング慢性的な無応答者の休止</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>マーケティングの慢性的なバウンスメールを中断</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>メールの更新後に「メールが無効です」をリセット</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>メールの更新後に「マーケティングが中断されました」をリセット</td>
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
