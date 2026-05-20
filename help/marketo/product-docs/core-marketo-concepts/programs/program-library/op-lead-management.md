---
description: リード管理運用プログラムテンプレート。 リードのライフサイクルとスコアリングの管理に利用できます。
title: OP-リード管理
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
TQID: https://experienceleague.adobe.com/KJvZjFZ9OsjIXXZTfbnscxf8puUxu-IxFXnNaj9JJFs
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
source-wordcount: 279
ht-degree: 16%

---

# OP-リード管理 {#op-lead-management}

この例では、Marketo Engageのデフォルトプログラムを使用して、Marketo Engage データベース内のレコードをCRMに管理する際に役立つ、リード管理のベストプラクティスワークフローを紹介します。

>[!NOTE]
>
>Marketo Engageでは、データベース内のレコードは人物/人物と呼ばれます。 この例でのリード管理は、CRMのレコードを参照しています。

詳しい戦略支援またはプログラムのカスタマイズに関するヘルプについては、Adobe アカウントチームにお問い合わせいただくか、[Adobe Professional Services](https://business.adobe.com/jp/customers/consulting-services/main.html) ページをご覧ください。

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
   <td>01 – 新規ユーザーをCRMに同期</td>
  </tr>
  <tr>
   <td>スマートキャンペーン</td>
   <td> </td>
   <td>02 - マーケティング適格</td>
  </tr>
  <tr>
   <td>メール</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">クイックスタートメールテンプレート</a></td>
   <td>01 - メール – アラート - MQL</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>キャンペーン</td>
  </tr>
  <tr>
   <td>フォルダー</td>
   <td> </td>
   <td>メールアラート</td>
  </tr>
 </tbody>
</table>

![](assets/op-lead-management-1.png)

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

* 組織で追跡している可能性のある各ライフサイクルステータスのニーズに対応するために、スマートキャンペーンを追加することを検討してください。 このプログラムで構築された各キャンペーンは、ベストプラクティスの構築の例となることを目的としており、すべてのユースケースに特化したものではありません。 そのため、特定のリードライフサイクル管理プロセスに対応するように、スマートキャンペーンを更新することが重要です。

* このプログラムの例の命名規則を、自分の例に合わせて更新することを検討してください。
