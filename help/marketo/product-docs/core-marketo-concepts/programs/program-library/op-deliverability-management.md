---
description: 配信性管理運用プログラムテンプレート。 メールの配信品質を維持するために使用します。
title: OP-配信品質管理
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
TQID: https://experienceleague.adobe.com/cJTv2uEq6YUEDphACUTypZOrkoLxTU0GRaPo43Igzjw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 19%

---

# OP-配信品質管理 {#op-deliverability-management}

これは、Marketo Engageのデフォルトプログラムを活用した配信品質管理のベストプラクティスワークフローの例です。メール配信の現状を確認し、慢性的なバウンスと非レスポンダーを管理します。

>[!NOTE]
>
>読み込むにはカスタム文字列フィールド「Marketing Suspended Reason」が必要です。 [詳細情報](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}。

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

## 前提条件フィールド {#prerequisite-fields}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>タイプ</th>
   <th>フレンドリ名</th>
   <th>API 名</th>
  </tr>
  <tr>
   <td>文字列</td>
   <td>マーケティングが中断された理由</td>
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
   <td>マーケティング部門が慢性的な無反応の人をサスペンドする</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>電子メールを定期的にバウンスしてマーケティングを中断</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>電子メールの更新後に「電子メールが無効」をリセット</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>電子メールの更新後に「マーケティングが中断されました」をリセット</td>
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
